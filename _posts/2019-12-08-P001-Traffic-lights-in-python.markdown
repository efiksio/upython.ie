---
layout: post
---
Thank you for watching my YouTube video.

You can find the upython sourde code from Traffic Light part 1 below:

{% highlight python %}
from pyb import Pin

red = Pin('X1', Pin.OUT_PP)
yellow = Pin('X2', Pin.OUT_PP)
green = Pin('X3', Pin.OUT_PP)

while True:
    green.high()
    pyb.delay(5000)
    green.low()
    yellow.high()
    pyb.delay(3000)
    yellow.low()
    red.high()
    pyb.delay(5000)
    red.low()
{% endhighlight %}

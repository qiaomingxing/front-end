# 移动Web开发

## 概述

移动web开发可以说是一个全新的领域，所遇到的问题跟PC端的web开发有很多的不同。

首先是浏览页面的场景不同导致的差异。在PC上，我们浏览网页最大的差异就是选用哪种浏览器，因此我们最多的是浏览器之间的兼容性。我们都知道移动设备种类繁多，我们需要考虑它们的系统（Andriod、ios、Android各种版本），它们屏幕尺寸，屏幕的物理分辨率等，而且移动设备的屏幕尺寸都比较小。总体而言，开发一个网页，我们就需要考虑不同系统的兼容性，设计的简洁性（不能像pc端一样内容那么复杂），适配各种尺寸和物理分辨率的屏幕。

不过庆幸地是，由于移动端的浏览器引擎大部分都是基于webkit的，这就可以大胆地使用HTML5的各种特性和API，这一点给开发带来了一定的便利。

其次，是交互上的不同。在PC上，与用户的交互大部分来源于鼠标的click事件。而在移动端，由于click历史原因导致的延迟，是不建议使用的，取而代之的是touch事件。我们用touch事件来模拟点击的行为，从而替代click事件。滚动也是用户在浏览网页经常进行的操作，而一个简单的滚动由于移动设备的不同会有各种问题。此外，我们还可以经常看到的下拉加载更多、上拉刷新等等移动设备特有的交互行为。

再有就是网络环境的差异。移动设备经常处于弱网的环境中，网速本来就慢，而且从移动设备发出的请求要经过层层转换才会到达互联网，之后再经过层层转换再回来，因此在http请求在移动端是最大的性能瓶颈，这一点要特别注意。

最后一个是移动设备自身的性能问题，一个再牛逼的手机，也不如一个普通的电脑的性能，因此在渲染页面的时候会比电脑的慢，很容易就会出现卡顿的现象，因此对于动画特效都要进行额外小心的设计和处理。

## 资源

1. [移动web入门](http://www.imooc.com/video/9579)
2. [如何构建mobile web项目](http://www.w3cplus.com/mobile/)
3. [mobile web基础](http://www.cnblogs.com/PeunZhang/p/3407453.html)
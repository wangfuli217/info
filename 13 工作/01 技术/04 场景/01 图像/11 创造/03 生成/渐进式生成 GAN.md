

# 渐进式生成 GAN

英伟达采取“渐进式生成”技术路线的 GAN 方案，这项方案的引人之处在于使得计算机可以生成 1024*1024大小的高清图片，它是目前无论图像清晰度还是图片生成质量都达到最好效果的技术，其生成的明星图片几乎可以达到以假乱真的效果。


<p align="center">
    <img width="70%" height="70%" src="http://images.iterate.site/blog/image/20190927/mlLPpyeuQIMw.png?imageslim">
</p>

> 英伟达提出渐进生成式 GAN 产生的高清头像图片

英伟达这项由粗到细，首先生成图像的模糊轮廓，再逐步添加细节的思想其实并非特别新颖的思路，在之前的 StackGAN 等很多方案都采用了类似思想，它的独特之处在于这种由粗到细的网络结构是动态生成的而非事先固定的静态网络，更关键的是产生的图片效果特别好。

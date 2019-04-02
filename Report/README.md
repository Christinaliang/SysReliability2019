1. 对于之前的想法（将判别器设置成一个多分类器）已经有类似的idea了[Improved Techniques for Training GANs](https://arxiv.org/abs/1606.03498)。

2. 对于最新的`GAN + semi-supervised + anomaly detection`方向的paper -- [GANomaly](https://arxiv.org/abs/1805.06725) 它的工作其实就是我们之前的工作，只不过没有优化loss function，而且它对半监督定义是“训练时用正常样本，这时就算监督学习了；然后测试时用正常和异常样本进行测试，这时属于非监督学习”。其次它的异常检测还是在图片集上面。具体细节写在paper summary.docx里面了。

3. 目前我所看到的将集成学习与GAN结合（这个方向倒是有很多将判别器设置为多分类器的模型）的paper都主要是为了解决`mode collapse`问题以及提高模型的鲁棒性而并没有没有涉及到异常检测。
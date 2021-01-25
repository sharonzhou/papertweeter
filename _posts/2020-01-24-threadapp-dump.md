---
layout: post
title: "My new paper with @NicolasPapernot and @GeoffreyHinton is out on arXiv today."
author: realSharonZhou
categories: [ Jekyll, tutorial ]
tags: [red, yellow]
image: "https://pbs.twimg.com/tweet_video_thumb/Dy0rL3kXQAEdQaz.jpg"
images: ["https://pbs.twimg.com/tweet_video_thumb/Dy0rL3kXQAEdQaz.jpg", "https://pbs.twimg.com/media/Dy0rjwEW0AATtSK.jpg", "https://pbs.twimg.com/media/Dy0rxTJXcAE-N_Q.jpg"]
---
<div class="t-main">
<div class="row t-tweet">
<div class="col-12">
<div id="tweet_1" class="content-tweet allow-preview" dir="auto">My new paper with <a class="entity-mention" href="https://twitter.com/NicolasPapernot">@NicolasPapernot</a> and <a class="entity-mention" href="https://twitter.com/geoffreyhinton">@GeoffreyHinton</a> is out on arXiv today. It's about the similarity structure of representations space, outlier data (e.g. adversarial attacks) and generative models. Don't have time to read the paper? Read this instead! <a class="entity-url" data-preview="true" href="https://arxiv.org/abs/1902.01889">arxiv.org/abs/1902.01889</a></div>
</div>
</div>
<div class="row t-tweet">
<div class="col-12">
<div id="tweet_2" class="content-tweet allow-preview" dir="auto">Our paper focused on a loss we call Soft Nearest Neighbor Loss (SNNL). It measures the entanglement of labeled data points. Data with high SNNL has muddled up classes, while the classes of a data set with low SNNL are easy to separate. <div class="entity-video-gif"><div class="vsc-controller" data-vscid="8aoqu5dr2"></div><video autoplay="" loop="" controls="" poster="https://pbs.twimg.com/tweet_video_thumb/Dy0rL3kXQAEdQaz.jpg" data-vscid="8aoqu5dr2"><source src="https://video.twimg.com/tweet_video/Dy0rL3kXQAEdQaz.mp4" type="video/mp4"><img alt="" src="https://pbs.twimg.com/tweet_video_thumb/Dy0rL3kXQAEdQaz.jpg"></video></div></div>
</div>
</div>
<div class="row t-tweet">
<div class="col-12">
<div id="tweet_3" class="content-tweet allow-preview" dir="auto">We can measure the SNNL of the data in the hidden layers of a resnet during training and show that each layer separates the data slightly more than the previous layer. the last layer learns a representation of the data which separates the classes, so it has the lowest SNNL value <div class="entity-image"><a href="https://pbs.twimg.com/media/Dy0rjwEW0AATtSK.jpg" target="_blank"><img alt="" src="https://pbs.twimg.com/media/Dy0rjwEW0AATtSK.jpg" class=" b-loaded"></a></div></div>
</div>
</div>
<div class="row t-tweet">
<div class="col-12">
<div id="tweet_4" class="content-tweet allow-preview" dir="auto">But entanglement can be desirable! You want the output of a GAN to be entangled with real data. If we measure the SNNL between real and generated data, we can see that SNNL increases over training. It serves as a good tool for understanding GAN training. <div class="entity-image"><a href="https://pbs.twimg.com/media/Dy0rxTJXcAE-N_Q.jpg" target="_blank"><img alt="" src="/images/1px.png" data-src="https://pbs.twimg.com/media/Dy0rxTJXcAE-N_Q.jpg"></a></div></div>
</div>
</div>
<div class="row t-tweet">
<div class="col-12">
<div id="tweet_5" class="content-tweet allow-preview" dir="auto">What happens if we learn a classifier by maximizing the SNNL of each hidden layer in addition to minimizing cross-entropy? We call these *Entangled Models* because their internal class representations are entangled. Surprisingly, this marginally increases performance! <div class="entity-image"><a href="https://pbs.twimg.com/media/Dy0sBGWW0AA7rI4.jpg" target="_blank"><img alt="" src="https://pbs.twimg.com/media/Dy0sBGWW0AA7rI4.jpg"></a></div></div>
</div>
</div>
<div class="row t-tweet">
<div class="col-12">
<div id="tweet_6" class="content-tweet allow-preview" dir="auto">Entangled models are better at detecting adversarial attacks using the DkNN. We estimate the uncertainty of each classification and find that entangled models project outlier data away from the expected manifold, making adversarial attacks easier to detect. <div class="entity-image"><a href="https://pbs.twimg.com/media/Dy0sMg-XcAE1H5r.jpg" target="_blank"><img alt="" src="https://pbs.twimg.com/media/Dy0sMg-XcAE1H5r.jpg"></a></div></div>
</div>
</div>
<div class="row t-tweet">
<div class="col-12">
<div id="tweet_7" class="content-tweet allow-preview" dir="auto">Entangled models are less vulnerable to black box attacks based on transferability. If we visualize the adversarial gradients of a targeted FGSM attack for normal models, we see shared class clusters. This enables transferability. These clusters don't exist with entangled models! <div class="entity-image"><a href="https://pbs.twimg.com/media/Dy0uBb4XgAAHU1f.jpg" target="_blank"><img alt="" src="https://pbs.twimg.com/media/Dy0uBb4XgAAHU1f.jpg"></a></div></div>
</div>
</div>
<div class="row t-tweet">
<div class="col-12">
<div id="tweet_8" class="content-tweet allow-preview" dir="auto">Entangled models arent trained with a specific attack in mind, so they should be good at distinguishing all outlier data from real data. If we train a model on MNIST and test it on notMIST, we see that entangled models project the outlier data far away from the real test data. <div class="entity-image"><a href="https://pbs.twimg.com/media/Dy0t-uHXgAEtLLv.jpg" target="_blank"><img alt="" src="https://pbs.twimg.com/media/Dy0t-uHXgAEtLLv.jpg"></a></div></div>
</div>
</div>
<div class="row t-tweet">
<div class="col-12">
<div id="tweet_9" class="content-tweet allow-preview" dir="auto">Read the paper for a more thorough investigation of this exciting loss and the effects of entangling classes in classifications networks and adversarial examples as well as an investigation of SNNL loss in GAN settings :) thanks for reading :)<br>
<a class="entity-url" data-preview="true" href="https://arxiv.org/abs/1902.01889">arxiv.org/abs/1902.01889</a></div>
</div>
</div>
</div>

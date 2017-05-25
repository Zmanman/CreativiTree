---
layout: default
title: Status
---

Progress Report
===============

[Source]: <> (http://sameersingh.org/courses/aiproj/sp17/writeups/status.pdf)

# Project Summary
[comment]: <> (Since things may have changed since proposal \(even if they haven’t\), write a short paragraph summarizing the goals of the project \(updated/improved version from the proposal\))
CreativiTree is fed thousands of images of trees using deep learning techniques in order to "hallucinate" new images of trees and then turning them into minecraft objects using malmo. 

# Approach
[comment]: <> (Give a detailed description of your approach, in a few paragraphs. You should summarize the main algorithm you are using, such as by writing out the update equation \(even if it is off-the-shelf\). You should also give details about the approach as it applies to your scenario. For example, if you are using reinforcement learning for a given scenario, describe the MDP in detail, i.e. how many states/actions you have, what does the reward function look like. A good guideline is to incorporate sufficient details so that most of your approach is reproducible by a reader. I encourage you to use figures, as appropriate, for this, as I provided in the writeup for the first assignment \(available here: http://sameersingh.org/courses/aiproj/sp17/assignments.html#assignment1\). I recommend at least 2-3 paragraphs.)

Following the orginal work of Ian Goodfellow on ["Generative Adverserial Networks"](https://arxiv.org/pdf/1406.2661.pdf), and consequently the work of several researchers from the University of Michigan on ["Generative Adversarial Text to Image Synthesis"](https://arxiv.org/pdf/1605.05396.pdf), this project focuses mainly on Image Systhesis \(Hallucinating Images\) and further explore its applications.

**The Learning**  
In order for CreativiTree to "learn" about trees, we used a TensorFlow implementation of Deep Convolutional Generative Adverserial Network (DCGAN) that we found on [github](https://github.com/carpedm20/DCGAN-tensorflow). This, along with thousands of 32x32 color tree images from the [CIFAR-100 dataset](https://www.cs.toronto.edu/~kriz/cifar.html).

**Hallucinating**


**Show Image here**

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

# Evaluation
[comment]: <> (An important aspect of your project, as we mentioned in the beginning, is evaluating your project. Be clear and precise about describing the evaluation setup, for both quantitative and qualitative results. Present the results to convince the reader that you have a working implementation. Use plots, charts, tables, screenshots, figures, etc. as needed. I expect you will need at least a few paragraphs to describe each type of evaluation that you perform.)


# Remaining Goals and Challenges
[comment]: <> (In a few paragraphs, describe your goals for the  next 2-3 weeks, when the final report is due. At the very least, describe how you consider your prototype to be limited, and what you want to add to make it a complete contribution. Note that if you think your algorithm is quite good, but have not performed sufficient evaluation, doing them can also be a reasonable goal. Similarly, you may propose some baselines \(such as a hand-coded policy\) that you did not get a chance to implement, but want to compare against for the final submission. Finally, given your experience so far, describe some of the challenges you anticipate facing by the time your final report is due, how crippling you think it might be, and what you might do to solve them.)

Our prototype currently uses an off the shelf DCGAN in order to perform image synthesis. Our main objective over the next 2-3 weeks is to code our own Generative Adversarial Neural Network and have more flexibility when it comes to improving its individual parts in order to hallucinate more realistic looking trees.

In addition, we would like to expand our DCGAN to generate images of objects other than trees. [write more]


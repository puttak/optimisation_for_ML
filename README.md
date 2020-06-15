# Nadam as a more polyvalent Adam with the increase of capacity in recurrent neural networks
In current state-of-the-art deep learning implementations, neural networks can have up to millions of parameters.  In addition, the loss to be optimized is almost always highly non-convex and therefore challenging to optimize. In the early days of deep learning, second-order methods, such as Hessian Free, were widely adopted to tackle these challenging problems. A bit later, first-order methods such as SGD were investigated with the intent of replacing second-order methods by using momentum and Nesterov accelerated gadient (NAG). Since then, throughout the years, research has focused on first-order methods for their simplicity and low computational cost. Since SGD, new first-order methods have emerged,  the most popular being Adam and RMSprop, with promises of greater performance. Adam, which is an extension of RMSprop with momentum is certainly performing well, but seems to struggle on certain problems where RMSprop delivers greater results. Indeed, momentum may impede the performance of Adam in specific cases, for instance when the difference in curvature varies between dimensions. A similar problem is described with classical momentum (CM). There, the authors propose to use NAG to achieve improved performance. In this paper, we investigate whether Nadam, a version of Adam incorporating NAG, gives more versatile results than Adam. Furthermore, Nadam is compared with RMSprop when Adam does not perform as well as the former. In particular, we examine how Nadam, RMSprop and Adam perform when the number of parameters, and thus the difficulty of the problem, changes. 

# Towards Deep and Efficient: A Deep Siamese Self-Attention Fully Efficient Convolutional Network for Change Detection in VHR Images
Change detection in multi-temporal very-high-resolution (VHR) images plays a significant role in facilitating the understanding of the relationships and interactions between human activities and the natural environment. Recently, fully convolutional networks (FCNs) have attracted widespread attention in the change detection field. In pursuit of better change detection performance, it has become a tendency to design deeper and more complicated FCNs, which inevitably brings about huge numbers of parameters and an unbearable computational burden. With the goal of designing a quite deep architecture to obtain more precise change detection results while simultaneously decreasing parameter numbers to improve efficiency, in this work, we present a very deep and efficient change detection network, entitled EffCDNet. In EffCDNet, to reduce the numerous parameters associated with deep architecture, an efficient convolution consisting of depth-wise convolution and group convolution with a channel shuffle mechanism is introduced to replace standard convolutional layers. In terms of the specific network architecture, EffCDNet does not use mainstream UNet-like architecture, but rather adopts another type of architecture with a very deep encoder and a lightweight decoder. In the very deep encoder, two very deep siamese streams stacked by efficient convolution first extract two highly representative and informative feature maps from input image-pairs. By performing a subtraction operation on two deep feature maps, a difference feature map containing rich change information is produced. Subsequently, an efficient atrous spatial pyramid pooling (EASPP) module is designed to capture multi-scale change information. In the lightweight decoder, a recurrent criss-cross self-attention (RCCA) module is applied to efficiently utilize non-local similar feature representations to enhance discriminability for each pixel, thus effectively separating the changed and unchanged regions. Moreover, to tackle the optimization problem in confused pixels, two novel loss functions based on information entropy are presented. On two challenging open change detection datasets, our approach outperforms other state-of-the-art FCN-based methods in terms of both visual interpretation and accuracy assessment, with only benchmark-level parameter numbers and quite low computational overhead, thereby demonstrating its effectiveness, superiority, and potential.

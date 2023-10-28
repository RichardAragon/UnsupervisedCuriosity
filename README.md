# UnsupervisedCuriosity
A Curiosity mechanism inspired by FARCuriosity but for unsupervised learning

Regarding Fragmentation: The choice of fragmentation technique would depend on the specific application being considered. In general, there are several ways to go about this:

1. Hierarchical Decomposition - This involves recursively dividing the environment into smaller subregions until a desired granularity level is reached. This approach can capture spatial dependencies within the environment and help reduce computational complexity since fewer interactions would occur between distant fragments. An example of this technique is called Multiscale Hilbert Space (MHS), where the space is divided into multiple scales based on distance between points.

2. Cluster Analysis - This involves finding groups of observations with similar properties through techniques such as K-means, DBSCAN, or HDBSCAN. Each cluster represents a distinct region in the environment, and local curiosity modules can be assigned to these clusters accordingly.

3. Unsupervised Segmentation Algorithms - There are many state-of-the-art approaches available for unsupervised segmentation of images or videos that could potentially serve as a basis for fragmenting environments in this context. These techniques typically employ deep neural networks trained on large datasets to learn features that enable semantic segmentation of input data. Examples include FCN (Fully Convolutional Networks), UNet (Upsampling Networks), and DeepLab v3+ (Pyramid Scene Parsing).

Assignment: After fragmentation, the next step would involve mapping local curiosity modules onto each fragment. One way to accomplish this could be to train separate local curiosity models for each fragment, and then choose the best performing model for each area. Alternatively, you could allocate resources dynamically based on the current state of each fragment, prioritizing areas that exhibit higher levels of uncertainty or novelty.

Updating Parameters: As mentioned earlier, there are various RL algorithms that can be employed to update parameter values in the local curiosity modules. Some popular options include Q-learning, Policy Gradient methods, and Actor Critic architectures.

Performance Evaluation: Although the authors don't provide results of their proposal on benchmark datasets or realistic problems, they argue that such an approach holds promise due to the ability to adapt to changing conditions and handle sparse rewards without supervision. They suggest that the framework could find practical applications in domains such as autonomous navigation, robotics, finance, and healthcare.

Some researchers have explored related ideas in recent years. For instance, the Soft Attention mechanism introduced in Transformers (Vaswani et al., 2017) enables selective feature extraction based on attention weights learned through training. Similarly, the DQfDQn framework presented in Oh et al. (2019) combines Decentralized Quantile Regression Forests with Deep Q-Networks to improve sample efficiency in reinforcement learning scenarios. More recently, in Fang et al. (2021), a hierarchical self-organization scheme was proposed to automate the design process of Deep Reinforcement Learning systems. It employs AutoML-like methods to automatically configure components of Deep RL architectures while incorporating domain knowledge when possible.

These works highlight the importance of addressing issues related to resource allocation, distributed computing, and scalability in complex decision-making tasks. While much remains to be done before the proposed framework becomes widely adopted, it offers promising insights into new directions for research in the intersection of Unsupervised Learning, Reinforcement Learning, and Multiagent Systems.

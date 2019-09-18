## Attack and Defence

Not only robust to noises, but robust the inputs that are built to fool the classifier.

**Training**(fixed inputs): Loss = C(y, y_true)
**Non-Targeted Attack** (fixed pre-trained parameters): Loss = -C(y', y_true)
**Targeted Attack**: Loss = -C(y', y_true) + C(y', y_false)

**With constraints: d(x,x') is not larger than a threshold**

constraints: 
L2-norm 
L-infinity : max{x}

Using Gradient Decent (With constraints)

# Attack Approaches:

FGSM (https://arxiv.org/abs/1412.6572)
Basic iterative method (https://arxiv.org/abs/1607.02533)
L-BFGS (https://arxiv.org/abs/1312.6199)
Deepfool (https://arxiv.org/abs/1511.04599)
JSMA (https://arxiv.org/abs/1511.07528)
C&W (https://arxiv.org/abs/1608.04644)
Elastic net attack (https://arxiv.org/abs/1709.04114)
Spatially Transformed (https://arxiv.org/abs/1801.02612)
One Pixel Attack (https://arxiv.org/abs/1710.08864)

Fast Gradient Sign Method (FGSM): sign(Gradient) -> can be seen as a model with very large learning rate.

**White Box Attack**:known network parameters

**Black Box Attack**: Train a proxy network yourself

Ref: Universal adversarial perturbations (https://arxiv.org/abs/1610.08401)

Ref: Adversarial Reprogramming of Neural Networks (https://arxiv.org/abs/1806.11146) fool the network to learn others


In real world, Find perturbations that generalize beyond a single image.(not one single angle)

---
##Defense 

#Passive defense: Finding the attached image without modifying the model (Special case of Anomaly Detection)

Add filter:

Smoothing

Feature Squeezing (https://arxiv.org/abs/1704.01155)

Randomization at Inference Phase (https://arxiv.org/abs/1711.01991)

#Proactive defense: Training a model that is robust to adversarial attack

Find the hull, make it up (add Adversarial samples to training set) [Data Augmentation]

Reference: https://adversarial-ml-tutorial.org/ (Zico Kolter and Aleksander Madry)

Adversarial Attack Toolbox:
• https://github.com/bethgelab/foolbox
• https://github.com/IBM/adversarial-robustness-toolbox
• https://github.com/tensorflow/cleverhans

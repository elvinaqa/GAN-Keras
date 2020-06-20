# GAN-Keras
Generative Adversarial Networks with Tensorflow Keras

2014  - Generative Adversarial Networks
2 networks competing against each other - counterfeiter and detector

Generator - generates random noise (ex: Gaussian Noise)
Discriminator - attempts to spot fake ones from real

Phase 1: Train Discriminator - labels real vs fake
Phase 2: Train Generator - produce better fake images 
![download (16)](https://user-images.githubusercontent.com/57037068/85209518-c6f2b200-b349-11ea-9c8f-468a87c3cd4c.png)


  Difficulties of GANs:
    Training Resources:
        CPU takes too long
            GPUs needed
            
    Mode Collapse:
        Producing same face since it already fools discriminator - thus, we need to have multiple images
            Deep Convolutional GANs - better for avoiding mode collapse; mini-batch discrimination - punishes similar imgs
    
    Instability:
        Difficulty of not being able to ascertain model's performance since it already produces sth fake
            Playing with hyperparameters changes the performance of model   
![download (15)](https://user-images.githubusercontent.com/57037068/85209519-c823df00-b349-11ea-9cf7-818df416810c.png)

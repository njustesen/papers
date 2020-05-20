# Reinforcement Learning

## Model-free RL

### PPO

### A2C

### DQN + variants

## Self-play

### Grandmaster level in StarCraft II using multi-agent reinforcement learning
Vinyals et al. (2019)

We chose to address the challenge of StarCraft using general-purpose learning methods that are in principle applicable to other complex domains: a multi-agent reinforcement learning algorithm that uses data from both human and agent games within a diverse league of continually adapting strategies and counter-strategies, each represented by deep neural networks5,6. We evaluated our agent, AlphaStar, in the full game of StarCraft II, through a series of online games against human players. AlphaStar was rated at Grandmaster level for all three StarCraft races and above 99.8% of officially ranked human players.

### Emergent Complexity vis Multi-agent Competition
Bansal et al. (2018)

We point out that a competitive multi-agent environment trained with self-play can produce behaviors that are far more complex than the environment itself. We also point out that such environments come with a natural curriculum, because for any skill level, an environment full of agents of this level will have the right level of difficulty.

## Exploration

### Go-Explore: a New Approach for Hard-Exploration Problems
Ecoffet et al. (2019)

We introduce a new algorithm called Go-Explore. It exploits the following principles: (1) remember states that have
previously been visited, (2) first return to a promising state (without exploration), then explore from it, and (3) solve simulated environments through exploiting any available means (including by introducing determinism), then robustify (create a policy that can reliably perform the solution) via imitation learning. The combined effect of these principles generates dramatic performance improvements on hardexploration problems. On Montezuma’s Revenge, without being provided any domain knowledge, Go-Explore scores over 43,000 points, almost 4 times the previous state of the art.

## Generalization / Regularization

### Rotation, Translation, and Cropping for Zero-Shot Generalization
Ye et al. (2020)

A growing mass of evidence suggests that these trained models fail to generalize to even slight variations of the environments they were trained on. This paper advances the hypothesis that the lack of generalization is partly due to the input representation, and explores how rotation, cropping and translation could increase generality. We show that a cropped, translated and rotated observation can get better generalization on unseen levels of a two-dimensional arcade game.

### Image Augmentation Is All You Need: Regularizing Deep Reinforcement Learning from Pixels
Kostrikov et al. (2020)

We propose a simple data augmentation technique that can be applied to standard model-free reinforcement learning algorithms, enabling robust learning directly from pixels without the need for auxiliary losses or pre-training. The approach leverages input perturbations commonly used in computer vision tasks to regularize the value function.

### Reinforcement Learning with Augmented Data
Laskin et al. (2020)

We present RAD: Reinforcement Learning with Augmented Data, a simple plug-and-play module that can enhance any RL algorithm. We show that data augmentations such as random crop, color jitter, patch cutout, and random convolutions can enable simple RL algorithms to match and even outperform complex state-of-the-art methods across common benchmarks in terms of data-efficiency, generalization, and wall-clock speed.

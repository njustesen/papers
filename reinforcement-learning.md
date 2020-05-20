# Reinforcement Learning

## Model-free RL

### PPO

### A2C

### DQN + variants

## Self-play

### Emergent Complexity vis Multi-agent Competition
Bansal et al. (2018)

We point out that a competitive multi-agent environment trained with self-play can produce behaviors that are far more complex than the environment itself. We also point out that such environments come with a natural curriculum, because for any skill level, an environment full of agents of this level will have the right level of difficulty.

## Curiosity-based RL

### Go-Explore: a New Approach for Hard-Exploration Problems
Ecoffet et al. (2019)

We introduce a new algorithm called Go-Explore. It exploits the following principles: (1) remember states that have
previously been visited, (2) first return to a promising state (without exploration), then explore from it, and (3) solve simulated environments through exploiting any available means (including by introducing determinism), then robustify (create a policy that can reliably perform the solution) via imitation learning. The combined effect of these principles generates dramatic performance improvements on hardexploration problems. On Montezuma’s Revenge, without being provided any domain knowledge, Go-Explore scores over 43,000 points, almost 4 times the previous state of the art.

## Input Augmentation/Modification

### Rotation, Translation, and Cropping for Zero-Shot Generalization
Ye et al. (2020)

A growing mass of evidence suggests that these trained models fail to generalize to even slight variations of the environments they were trained on. This paper advances the hypothesis that the lack of generalization is partly due to the input representation, and explores how rotation, cropping and translation could increase generality. We show that a cropped, translated and rotated observation can get better generalization on unseen levels of a two-dimensional arcade game.

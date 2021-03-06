# Reinforcement Learning

## Model-free RL

### SEED RL: Scalabel and Efficient Deep-RL and with Accelerated Central Inference
Espeholt et al. (2020)

We show that it is not only possible to train on millions of frames per second but also to lower the cost of experiments compared to current methods. We achieve this with a simple architecture that features centralized inference and an optimized communication layer. SEED adopts two state of the art distributed algorithms, IMPALA/V-trace (policy gradients) and R2D2 (Q-learning), and is evaluated on Atari-57, DeepMind Lab and Google Research Football.

### Agent57: Outperforming the Atari Human Benchmark
Badia et al. (2020)

We propose Agent57, the first deep RL agent that outperforms the standard human benchmark on all 57 Atari games. To achieve this result, we train a neural network which parameterizes a family of policies ranging from very exploratory to purely exploitative. We propose an adaptive mechanism to choose which policy to prioritize throughout the training process. Additionally, we utilize a novel parameterization of the architecture that allows for more consistent and stable learning.

### Implementation Matters in Deep RL: A Case Study on PPO and TRPO
Engstrom et al. (2019)

We study the roots of algorithmic progress in deep policy gradient algorithms through a case study on two popular algorithms: Proximal Policy Optimization (PPO) and Trust Region Policy Optimization (TRPO). Specifically, we investigate the consequences of "code-level optimizations:" algorithm augmentations found only in implementations or described as auxiliary details to the core algorithm. Seemingly of secondary importance, such optimizations turn out to have a major impact on agent behavior. Our results show that they (a) are responsible for most of PPO's gain in cumulative reward over TRPO, and (b) fundamentally change how RL methods function.

*Related resources:*
https://costa.sh/blog-the-32-implementation-details-of-ppo.html

### Proximal Policy Optimization Algorithms
Schulman et al. (2017)

We propose a new family of policy gradient methods for reinforcement learning, which alternate between sampling data through interaction with the environment, and optimizing a "surrogate" objective function using stochastic gradient ascent. Whereas standard policy gradient methods perform one gradient update per data sample, we propose a novel objective function that enables multiple epochs of minibatch updates. The new methods, which we call proximal policy optimization (PPO), have some of the benefits of trust region policy optimization (TRPO), but they are much simpler to implement, more general, and have better sample complexity (empirically).

### Asynchronous Methods for Deep Reinforcement Learning
Mnih et al. (2016)

We propose a conceptually simple and lightweight framework for deep reinforcement learning that uses asynchronous gradient descent for optimization of deep neural network controllers. We present asynchronous variants of four standard reinforcement learning algorithms and show that parallel actor-learners have a stabilizing effect on training allowing all four methods to successfully train neural network controllers.

### Trust Region Policy Optimization
Schulman et al. (2015)

We describe an iterative procedure for optimizing policies, with guaranteed monotonic improvement. By making several approximations to the theoretically-justified procedure, we develop a practical algorithm, called Trust Region Policy Optimization (TRPO). This algorithm is similar to natural policy gradient methods and is effective for optimizing large nonlinear policies such as neural networks.

### Playing Atari with Deep Reinforcement Learning
Mnih et al. (2013)

Also published in Nature: "Human-level control through deep reinforcement learning" (2015)

We present the first deep learning model to successfully learn control policies directly from high-dimensional sensory input using reinforcement learning. The model is a convolutional neural network, trained with a variant of Q-learning, whose input is raw pixels and whose output is a value function estimating future rewards.

## Self-play

### SCC: An Efficient Deep Reinforcement Learning Agent Mastering the Game of StarCraft II
Wang et al. (2020)

We propose a deep reinforcement learning agent, StarCraft Commander (SCC). With order of magnitude less computation, it demonstrates top human performance
defeating GrandMaster players in test matches and top professional players in a live event. Moreover, it shows strong robustness to various human strategies and
discovers novel strategies unseen from human plays

### Grandmaster level in StarCraft II using multi-agent reinforcement learning
Vinyals et al. (2019)

We chose to address the challenge of StarCraft using general-purpose learning methods that are in principle applicable to other complex domains: a multi-agent reinforcement learning algorithm that uses data from both human and agent games within a diverse league of continually adapting strategies and counter-strategies, each represented by deep neural networks5,6. We evaluated our agent, AlphaStar, in the full game of StarCraft II, through a series of online games against human players. AlphaStar was rated at Grandmaster level for all three StarCraft races and above 99.8% of officially ranked human players.

### Emergent Complexity vis Multi-agent Competition
Bansal et al. (2018)

We point out that a competitive multi-agent environment trained with self-play can produce behaviors that are far more complex than the environment itself. We also point out that such environments come with a natural curriculum, because for any skill level, an environment full of agents of this level will have the right level of difficulty.

### Deep Reinforcement Learning from Self-Play in Imperfect-Information Games
Heinrich et al. (2016)

We introduce the first scalable end-to-end approach to learning approximate Nash equilibria without prior domain knowledge. Our method combines fictitious self-play with deep reinforcement learning.

## Exploration

### QD-RL: Efficient Mixing of Quality and Diversity in Reinforcement Learning
Cideron et al. (2020)

We train a population of off-policy deep RL agents to simultaneously maximize
diversity inside the population and the return of the agents. QD-RL selects agents
from the diversity-return Pareto Front, resulting in stable and efficient population
updates. Our experiments on the ANT-MAZE environment show that QD-RL can
solve challenging exploration and control problems with deceptive rewards while
being more than 15 times more sample efficient than its evolutionary counterparts.

### First return then explore
Ecoffet et al. (2020)

We hypothesise that the main impediment to effective exploration originates from algorithms forgetting how to reach previously visited states (“detachment”) and from failing to first return to a state before exploring from it (“derailment”). We introduce Go-Explore, a family of algorithms that addresses these two challenges directly through the simple principles of explicitly remembering promising states and first returning to such states before intentionally exploring. Go-Explore solves all heretofore unsolved Atari games (meaning those for which algorithms could not previously outperform humans when evaluated following current community standards for Atari and surpasses the state of the art on all hard-exploration games.

### Go-Explore: a New Approach for Hard-Exploration Problems
Ecoffet et al. (2019)

We introduce a new algorithm called Go-Explore. It exploits the following principles: (1) remember states that have
previously been visited, (2) first return to a promising state (without exploration), then explore from it, and (3) solve simulated environments through exploiting any available means (including by introducing determinism), then robustify (create a policy that can reliably perform the solution) via imitation learning. The combined effect of these principles generates dramatic performance improvements on hardexploration problems. On Montezuma’s Revenge, without being provided any domain knowledge, Go-Explore scores over 43,000 points, almost 4 times the previous state of the art.

### Exploration by Random Network Destillation
Burda et al. (2018)

We introduce an exploration bonus for deep reinforcement learning methods that is easy to implement and adds minimal overhead to the computation performed. The bonus is the error of a neural network predicting features of the observations
given by a fixed randomly initialized neural network.

### Deep Reinforcement Learning from Human Preferences
Christiano et al. (2017)

We explore goals defined in terms of (non-expert) human preferences between pairs of trajectory segments. We show that this approach can effectively solve complex RL tasks without access to the reward function.

## Generalization / Regularization

### Rotation, Translation, and Cropping for Zero-Shot Generalization
Ye et al. (2020)

This paper advances the hypothesis that the lack of generalization is partly due to the input representation, and explores how rotation, cropping and translation could increase generality. We show that a cropped, translated and rotated observation can get better generalization on unseen levels of a two-dimensional arcade game.

### Image Augmentation Is All You Need: Regularizing Deep Reinforcement Learning from Pixels
Kostrikov et al. (2020)

We propose a simple data augmentation technique that can be applied to standard model-free reinforcement learning algorithms, enabling robust learning directly from pixels without the need for auxiliary losses or pre-training. The approach leverages input perturbations commonly used in computer vision tasks to regularize the value function.

### Reinforcement Learning with Augmented Data
Laskin et al. (2020)

We present RAD: Reinforcement Learning with Augmented Data, a simple plug-and-play module that can enhance any RL algorithm. We show that data augmentations such as random crop, color jitter, patch cutout, and random convolutions can enable simple RL algorithms to match and even outperform complex state-of-the-art methods across common benchmarks in terms of data-efficiency, generalization, and wall-clock speed.

### Paired Open-Ended Trailblazer (POET): Endlessly Generating Increasingly Complex and Diverse Learning Environments and Their Solutions
Wang et al. (2019)

While the history of machine learning so far largely encompasses a series of problems posed by researchers and algorithms that learn their solutions, an important question is whether the problems themselves can be generated by the algorithm at the same time as they are being solved. Such a process would in effect build its own diverse and expanding curricula, and the solutions to problems at various stages would become stepping stones towards solving even more challenging problems later in the process. The Paired Open-Ended Trailblazer (POET) algorithm introduced in this paper does just that: it pairs the generation of environmental challenges and the optimization of agents to solve those challenges. It simultaneously explores many different paths through the space of possible problems and solutions and, critically, allows these stepping-stone solutions to transfer between problems if better, catalyzing innovation. 

## Model-based RL

### Mastering Atari with Discrete World Models
Hafner et al (2020)

We introduce DreamerV2, a reinforcement learning agent that learns behaviors purely from predictions in the compact latent space of a powerful world model. The world model uses discrete representations and is trained separately from the policy. DreamerV2 constitutes the first agent that achieves human-level performance on the Atari benchmark of 55 tasks by learning behaviors inside a separately trained world model.

### Planning to Explore via Self-Supervised World Models
Sekar et al (2020)

We present Plan2Explore, a self-supervised reinforcement learning agent that tackles both these challenges through a new approach to self-supervised exploration and fast adaptation to new tasks, which need not be known during exploration. During exploration, unlike prior methods which retrospectively compute the novelty of observations after the agent has already reached them, our agent acts efficiently by leveraging planning to seek out expected future novelty.

### Deployment-Efficient Reinforcement Learning via Model-Based Offline Optimization
Matsushima et al. (2020)

We propose a novel model-based algorithm, Behavior-Regularized Model-ENsemble (BREMEN) that can effectively optimize a policy offline using 10-20 times fewer data than prior works. Furthermore, the recursive application of BREMEN is able to achieve impressive deployment efficiency while maintaining the same or better sample efficiency, learning successful policies from scratch on simulated robotic environments with only 5-10 deployments, compared to typical values of hundreds to millions in standard RL baselines.

### Dream to Control: Learing Behaviors by Latent Imagination
Hafner et al. (2020)

We present Dreamer, a reinforcement learning agent that solves long-horizon tasks from images purely by latent imagination. We efficiently learn behaviors by propagating analytic gradients of learned state values back through trajectories imagined in the compact state space of a learned world model. 

### World Models
Ha & Schmidhuber (2018)

We explore building generative neural network models of popular reinforcement learning environments. Our world model can be trained quickly in an unsupervised manner to learn a compressed spatial and temporal representation of the environment. By using features extracted from the world model as inputs to an agent, we can train a very compact and simple policy that can solve the required task. We can even train our agent entirely inside of its own hallucinated dream generated by its world model, and transfer this policy back into the actual environment.

## Unsupervised

### Emergent Real-World Robotic Skills via Unsupervised Off-Policy Reinforcement Learning
Sharma et al. (2020)

We demonstrate that a recently proposed unsupervised skill discovery algorithm can be extended into an efficient off-policy method, making it suitable for performing unsupervised reinforcement learning in the real world. 

## Offline RL

### Offline Reinforcement Learning: Tutorial, Review, and Perspectives on Open Problems
Levine et al. (2020)

We aim to provide the reader with the conceptual tools needed to get started on research on offline reinforcement learning algorithms: reinforcement learning algorithms that utilize previously collected data, without additional online data collection.

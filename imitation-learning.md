# RL-based IL

## Recall Traces: Backtracking Models for Efficient Reinforcement Learning
Goyal et al. (2019)

We advocate for the use of a backtracking model that predicts the preceding states that terminate at a given high-reward state. We can train a model which, starting from a high value state (or one that is estimated to have high value), predicts and samples which (state, action)-tuples may have led to that high value state. These traces of (state, action) pairs, which we refer to as Recall Traces, sampled from this backtracking model starting from a high value state, are informative as they terminate in good states, and hence we can use these traces to improve a policy.

## Learning Montezuma’s Revenge from a Single Demonstration
Salimans & Chen (2018)

We propose a new method for learning from a single demonstration to solve hard exploration tasks like the Atari game Montezuma’s Revenge. Instead of imitating
human demonstrations, as proposed in other recent works, our approach is to maximize rewards directly. Our agent is trained using off-the-shelf reinforcement learning, but starts every episode by resetting to a state from a demonstration.

## Self-Imitation Learning
Oh et al. (2018)

We propose a Self-Imitation Learning (SIL) algorithm which learns to imitate the agent’s own past good decisions. In brief, the SIL algorithm stores experiences in a replay buffer, learns to imitate state-action pairs in the replay buffer only when the return in the past episode is greater than the agent’s value estimate. 

## Deep Q-learning from Demonstrations
Hester et al. (2017)

We study a setting where the agent may access data from previous control of the system. We present an algorithm, Deep Q-learning from Demonstrations (DQfD), that leverages small sets of demonstration data to massively accelerate the learning process even from relatively small amounts of demonstration data and is able to automatically assess the necessary ratio
of demonstration data while learning thanks to a prioritized replay mechanism.

# Diversity-based IL

## BRIL

## GAIL

## InfoGAIL



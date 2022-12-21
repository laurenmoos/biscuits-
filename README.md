branching condition

What would work best for all of you?

###RL learning through human feedback

this differs from conventional RL in the sense that there is not a pre-specified goal, instead a (human) reverse engineer periodically guides learning 

1. Periodically, a batch of behaviors (episodes/finite state machines/sequences  of (S, A) with A  high-level UX actions and S  consisting of heap in use data and heap regularization data returned from Cannoli is sent to a human reverse engineer who is asked to select which one shows the best steps towards a desired goal. Note: this also lets episodes be further decomposed into behaviors, or subsequences of an episode.
2. The human's choice is used to train a reward predictor which trains an agent. The agent learns to maximize the reward from the predictor


### learning via indirect human feedback

similar to 1) there is not a conventional reward function and instead recovers an expert's cost function but unlike 1) it does this with example behaviors at the start of training and a generative model that learns to augment them 

In this case, behaviors (sub-sequences of the same response object described in 1. and available during training) are collected prior to program run

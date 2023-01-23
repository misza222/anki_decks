# Unit 5 of HF RL Course

## Policy-gradient methods

Policy is changed directly. It is stored in a neural network and updated upon completed episodes using gradient-ascent

## Reinforce

Policy-gradient method where at the end of the episode probability of taking each step is boosted if episode was successfull or vice-versa. This boosting is proportional to the value of the final reward at the end of the episode.

## Reinforce problems
 * high variance because of the stochasticity of the policy: because of the randomness in the environment and quasi-random<sup>1</sup> in the policy itself, simillar trajectories can lead to different outcomes. 

<sub>1. Quasi-random, as it is still based on a policy that with time learns better and better to choose right moves (distribution for the next action is showing the clean "winner action") where and when it matters.</sub>
 
## Monte-carlo sampling

In Policy-gradient it means sampling entire episode and creating trajectory τ. The process is not entirely random, as it is using the current policy to return distribution of actions at each step, but then the action is drawn from that distribution.


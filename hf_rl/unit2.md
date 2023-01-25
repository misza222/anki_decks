# Unit 2 of HF RL Course

## Temporal difference (TD)
Learning happens after each step taken by the agent

For example computing non discounted value of a state using TD learning:
V(s<sub>t</sub>) = V(s<sub>t</sub>) + &alpha; * ( R<sub>t+1</sub> - V(S<sub>t+1</sub>) + V(S<sub>t</sub>) )

## Monte Carlo Learning
Learning takes place at the end of the episode and entire trajectory &tau; is used (e.g. policy-gradient method)

For example computing non discounted value of a state using Monte carlo learning:
V(s<sub>t</sub>) = V(s<sub>t</sub>) + &alpha; * ( G<sub>t</sub> - V(S<sub>t</sub>) ), where G is empirical return from the episode


## Bellman equation

Value of the state given policy &pi; equals:
V(s<sub>t</sub>) = R<sub>t+1</sub> + &gamma; * V(S<sub>t+1</sub>)

![Bellman equation](bellman_eq_1.jpeg)

## Q-Learning

Off-policy Temporal Difference learning approach that is using value-based method. Internally it is using a table for all the (action,state) tuples and assigns them a value.

## on-policy
Update algorithm that is using the same policy for acting and updating

## off-policy
Update algorithm that is using one policy for acting and another one for updating
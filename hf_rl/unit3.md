# Unit 3 of HF RL Course

## Problems with Q-Learning

It is memmory inefficient as for each (state, action) it requires a separate entry in the table. For environments with high number of states and/or long/infinite horizon it is impossible to do that.

## Deep Q-Networks (DQN)

Mechanism of (lossy) compressing Q-Learning table into a NN. For a given (state, action) it returns a probability distribution over possible actions. Actions with high probability are more likely to achieve better results.

## Temporal limitation

Limitation of environments where using a single observation it is impossible to figure out all the properties of observed objects. For example when we get frames from the video game, we have to use at least 2 frames to figure out direction and velocity of an object.

## Experience replay

## Deep Q-Learning algorithm
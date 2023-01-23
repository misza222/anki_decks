# Unit 6 of HF RL Class

## Acrot-Critic

Hybrid architecure combining value-based and policy-based methods:
 - an *Actor* controls how our agent behaves
 - a *Critic* that measures how good the taken action is

In comparison with Policy-gradient method, it helps to stalilize the training by reducing the variance.

## Actor algorithm
* performs an action, letting the critic know


## Critic algorithm
* Given A<sub>t</sub> chosen by the Actor it performs it's estimation of the Q-value using function q_hat(S<sub>t</sub>, A<sub>t</sub>)
* Observing state S<sub>t+1</sub> and reward R<sub>t+1</sub> it updates it's model for computing q_hat (parametrized with *w*):
  delta_w = beta * TD Error * w_grad, where the loss function is a *TD Error = R(S<sub>t</sub>, A<sub>t</sub>) + epsilon*q_hat(S<sub>t+q</sub>, A<sub>t+1</sub>) - q_hat(S<sub>t</sub>, A<sub>t</sub>)*

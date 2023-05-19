# Qualification project - RL in Ubran Mobility

> This excercise is intended for candidates for PhD students in COeXISTENCE
> 
> Please send the solution reports to coexistence@uj.edu.pl

---

![image](https://user-images.githubusercontent.com/20555451/238653204-e8af9e52-262b-493b-a931-5cb3695bebd2.png)


1. Let's consider set of $Q$ individual travellers want to reach from their origin $O$ to their destination $D$.
2. Everyday they choose between the two alternative routes: $a$ and $b$.
3. The cost (travel time) is given with a naive, non-linearly increasing `BPR` formula:

$t_a(q_a) = t^0_a (1 + (q_a / Q_a)^2)$, 

where:

* $t_a(q_a)$ - is the travel time on arc a (or b)
* $q_a$ - is the flow (number of vehicles using arc)
* $t^0_a$ - is the free flow speed (with no other vehicles)
* $Q_a$ - is the capacity (maximal number of vehices)


4. Let's consider the following parameterization:

* $Q$ = 1000 veh
* $t^0_a$ = 5 min
* $t^0_b$ = 15 min
* $Q_a$ = 500 veh/h
* $Q_b$ = 800 veh/h

--- 

### Tasks:
1. Compute (analytically) the `System Optimum` and `User Equilibrium` of such system, 
 * System Optimum is the solution where total costs are minimised: 
 
  $t_a(q_a)* q_b + t_b(q_b) * q_b$, s.t. $q_a + q_b = Q$ , $q_a, q_b \geq 0$
 * User Equilibrium is the system where each traveller is individually satisfied, i.e. $t_a(q_a) = t_b(q_b)$

2. Now let's reforumulate the above as `Reinforcement Learning`, i.e. each agent (traveller) every day makes a decision which path to take to maximise her reward.
3. Implement and solve the RL problems which find the SO and UE resepctively.
4. Propose the centralized solution, where all the actions are taken jointly (coordinated).
5. As well as decentralized (`MARL`) where each agent independently makes her decisions.
6. Comment on the problem: formulation, complexity, convergence, algorithms used, reward functions, etc.

----
(c) Rafał Kucharski, 2023
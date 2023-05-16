# Qualification project - RL in Ubran Mobility

> This excercise is intended for candidates for PhD students in COeXISTENCE
> 
> Please send the solution reports to coexistence@uj.edu.pl

1. Let's consider set of $Q$ individual travellers want to reach from origin $O$ to destination $D$.
2. The have two alternatives $a$ and $b$
3. The cost (travel time)  is given with a naive, non-linearly increasing `BPR` formula:

$t_a(q_a) = t^0_a (1 + (q_a / Q_a)^2)$, 

where:

$t_a(q_a)$ - is the travel time on arc a (or b)
$q_a$ - is the flow (number of vehicles using arc
$t^0_a$ - is the free flow speed (with no other vehicles)
$Q_a$ - is the capacity (maximal number of vehices)

4. Each traveller is free to choose between alternatives everyday.
5. Compute the `System Optimum` and `User Equilibrium` of such system, 
 * System Optimum is the solution where total costs are minimised ($t_a(q_a)* q_b + t_b(q_b) * q_b$, s.t. $q_a>0 + q_b>0




![image](https://user-images.githubusercontent.com/20555451/238649487-9974e36e-1464-408c-b8b4-9287bfb15d70.png)



(c) Rafał Kucharski, 2023
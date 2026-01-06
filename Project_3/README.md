# Finding the Optimal Racing Path using Monte Carlo Methods

In this problem, a racing car must move from a starting line to a finish line on a discrete racetrack grid.  
The objective is to reach the finish line in minimum time.

The racetrack is represented as a grid of valid cells. At each step, the car has a position (x, y) and a velocity (vx, vy).

---

## Environment Rules

- At each time step, the car can change each velocity component by:
  - −1, 0, or +1
- Velocity constraints:
  - 0 ≤ vx < 5  
  - 0 ≤ vy < 5  
  - (vx, vy) cannot both be zero except at the starting line
- The car moves according to its velocity:
  - New position = (x + vx, y + vy)

---

## Rewards

- Each step gives a reward of **−1**
- Reaching the finish line ends the episode
- If the car hits the wall or leaves the track:
  - Reward = −5  
  - The car is reset to a random starting position  
  - Velocity is reset to (0, 0)  
  - The episode continues

---

## Episode Definition

- Each episode starts from a random starting cell on the starting line with velocity (0, 0)
- The episode ends when the car crosses the finish line

---

## Task

Use the On-policy First-Visit Monte Carlo Control (ε-soft) algorithm to estimate the optimal policy π*.

Implement the algorithm in Python (as described in the textbook, page 101), and visualize the optimal trajectories for 6 different starting cells on the starting line.



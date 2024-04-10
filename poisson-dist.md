### Problem
Is it optimal for a police car to drive around a neighborhood to find traffic violations or to stay at a single position and monitor one location?

### Solution
Let's simplify the problem: considering two intersections, each with rates of traffic violations over a given time frame, and one police car, is it more optimal for an officer to observe one location for a period of time or move between both locations? 

Let's gather the parameters of the problem:
1. there is 1 officer (the observer)
2. there are 2 locations, point A and point B
3. each location has a probability rate of traffice violations per hour: let's assume each is the same at 10 violations per hour

In order to solve this problem, we will have to use a poisson distribution. The Poisson distribution deals with the frequency with which an event occurs within a specific interval. 

```math
\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
```

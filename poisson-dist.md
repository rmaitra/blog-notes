### Problem
Is it optimal for a police car to drive around a neighborhood to find traffic violations or to stay at a single position and monitor one location?

### Solution
Let's simplify the problem: considering two intersections, each with rates of traffic violations over a given time frame, and one police car, is it more optimal for an officer to observe one location for a period of time or move between both locations? 

Let's gather the parameters of the problem:
1. there is 1 officer (the observer)
2. there are 2 locations, point A and point B
3. each location has a mean probability rate of traffice violations per hour: let's assume each is the same at a mean rate of 10 violations per hour

In order to solve this problem, we will have to use a poisson distribution. The Poisson distribution deals with the frequency with which an event occurs within a specific interval. The poisson distribution is as follows:

```math
P(X) = { e^{-\lambda} \lambda^k \over k! }
```

Where:
- $P(X)$ is the probability that the officer will observe a traffic violation
- $e$ is Euler's constant
- $\lambda$ is the mean of the outcome
- $k$ is the number of event occurences  


Is the probability of observing a traffic violation higher if the officer splits time between two locations or stays at the same location?

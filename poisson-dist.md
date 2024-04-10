### Problem
Is it optimal for a police car to drive around a neighborhood to find traffic violations or to stay at a single position and monitor one location?

### Solution
Let's simplify the problem: considering two intersections, each with rates of traffic violations over a given time frame, and one police car, is it more optimal for an officer to observe one location for a period of time or move between both locations? 

Let's gather the parameters of the problem:
1. there is 1 officer (the observer)
2. there are 2 locations, point A and point B
3. there is a 10% chance of a violation occurring at each location per hour

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

The probability of seeing at least 1 violation at point A location over 10 hours is:
```math
P(A)=1-(P_{no-violation})^{t}
```
```math
P_{no-violation} = 1 - 0.1 = 0.9
```
```math
t = 10
```
```math
P(A) = 1-(0.9)^{10} = 0.651
```
There's a 65.1% chance of observing a violation at one location (in this instance point A) if the officer spends all 10 hours there.

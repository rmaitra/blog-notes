### Problem
Is it optimal for a police car to drive around a neighborhood to find traffic violations or to stay at a single position and monitor one location?

### Solution
Let's simplify the problem: considering two intersections, each with rates of traffic violations over a given time frame, and one police car, is it more optimal for an officer to observe one location for a period of time or move between both locations? 

Let's gather the parameters of the problem:
1. there is 1 officer (the observer)
2. there are 2 locations, point A and point B
3. each location has a probability rate of traffice violations per hour: let's assume each is the same at 10 violations per hour
4. the officer has a 10 hour timeframe to be at either point A and/or B (e.g. 9 hours at A and 1 hour at B, or 10 hours at B and 0 hours at A)

In order to solve this problem, we will have to use a poisson distribution. The Poisson distribution deals with the frequency with which an event occurs within a specific interval. 

```math
P(X) = { e^{-\lambda} \lambda^k \over k! }
```
Where:
- $P(X)$ is the probability that the officer will observe a traffic violation
- $e$ is Euler's constant
- $\lambda$ is the mean of the outcome
- $k$ is the number of occurences

If the officer stays at 1 location (A or B) for the whole 10 hours, the officer will observe 10 violations per hour.
If the officer moves between both locations, will the officer observe more, the same or less than 10 violations per hour?

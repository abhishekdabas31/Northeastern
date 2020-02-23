# Poisson Process
A Poisson Process is a model for a series of discrete event where the average time between events is known, but the exact timing of events is random. The arrival of an event is independent of the event before (waiting time between events is memoryless). For example, suppose we own a website which our content delivery network (CDN) tells us goes down on average once per 60 days, but one failure doesn’t affect the probability of the next. All we know is the average time between failures

## The important point is we know the average time between events but they are randomly spaced (stochastic). We might have back-to-back failures, but we could also go years between failures due to the randomness of the process.
A Poisson Process meets the following criteria (in reality many phenomena modeled as Poisson processes don’t meet these exactly):
Events are independent of each other. The occurrence of one event does not affect the probability another event will occur.
The average rate (events per time period) is constant.
Two events cannot occur at the same time.

### Common examples of Poisson processes are customers calling a help center, visitors to a website, radioactive decay in atoms, photons arriving at a space telescope, and movements in a stock price. Poisson processes are generally associated with time, but they do not have to be. In the stock case, we might know the average movements per day (events per time), but we could also have a Poisson process for the number of trees in an acre (events per area).

# Poisson Distribution
The Poisson Process is the model we use for describing randomly occurring events and by itself, isn’t that useful. We need the Poisson Distribution to do interesting things like finding the probability of a number of events in a time period or finding the probability of waiting some time until the next event.

This is a little convoluted, and events/time * time period is usually simplified into a single parameter, λ, lambda, the rate parameter. With this substitution, the Poisson Distribution probability function now has one parameter

Lambda can be thought of as the expected number of events in the interval. (We’ll switch to calling this an interval because remember, we don’t have to use a time period, we could use area or volume based on our Poisson process). I like to write out lambda to remind myself the rate parameter is a function of both the average events per time and the length of the time period but you’ll most commonly see it as directly above.

## The most likely number of events in the interval for each curve is the rate parameter. This makes sense because the rate parameter is the expected number of events in the interval and therefore when it’s an integer, the rate parameter will be the number of events with the greatest probability.

When it’s not an integer, the highest probability number of events will be the nearest integer to the rate parameter, since the Poisson distribution is only defined for a discrete number of events. The discrete nature of the Poisson distribution is also why this is a probability mass function and not a density function. (The rate parameter is also the mean and variance of the distribution, which do not need to be integers.)


Source:- 
1. https://towardsdatascience.com/the-poisson-distribution-and-poisson-process-explained-4e2cb17d459
# 27 March 2025 

A few things I want to accomplish here: 

* Figure out how variable infectiousness periods are in the NBA study, assuming some kind of simple threshold model. 
* Figure out how this relates to PCR detectability -- e.g., set infectiousness at Ct=30, detectability at Ct=40. How quickly do we reach infectiousness? 

Maybe it'd be worth considering two thresholds of infectiousness -- something like low-level and high-level infectiousness, roughly corresponding to the possibility of transmission to close contacts vs. superspreading? We don't know where exactly those thresholds would be (and surely there aren't strict thresholds), but it might be useful for illustration. 

I can already think of some important extensions: how much does our commitment to the tent model matter? I imagine there are some people that might linger above the high infectiousness threshold, but the tent model can't capture that behavior and artificially shortens the time spent at high infectiousness. 

Maybe it's worth treating **screening** and **isolation** separately & independently. Given a screening rate, how many infections do we miss when there's heterogeneity in the proliferation period? Given an isolation period, how many infectious people are released -- and how many days of unnecessary isolation are there -- for a fixed isolation period? How much do we gain by testing twice? How does additional surveillance help us understand the risks associated with our policy choices? 

Characterizing in terms of the proliferation rate might make sense here -- even though fitting to the proliferation time is easier. 

# 28 March 2025 

Some things I want to get done before next week: 
* Simulate outbreaks under a given screening and isolation policy, for different levels of variation in the proliferation and clearance phases. 

An algorithm:
* Set thresholds for detectability and infectiousness
* Generate N trajectories 
* Reduce trajectories to timings of detectability and infectiousness 
* Set a screening rate and isolation period 
* Simulate epidemics under different assumptions about variation in timing of infectiousness/etc 

Given this information, separate out the number of people we don't isolate before infectious, the number of people taht leave isolation while infectious, the number of people who isolate unnecesarily, the size of the epidemic (maybe) 


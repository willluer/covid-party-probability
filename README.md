# covid-party-probability


## Definitions:
$$ P(-): \text{Probability of one person being negative}$$
$$ P(+): \text{Probability of one person being positive}$$
$$ N: \text{Number of people at the event}$$
$$ population\ size: \text{County population}$$
$$ \#\ positive\ cases: \text{Number of reported and unreported positive cases in a specific population}$$
$$ FS: \text{Factor of safety}$$
$$ incubation\ period: \text{Length of time in which a person is unknowingly positive}$$   

  
## Derivation:

**The population wide probability of being positive can be estimated by dividing the number of positive cases within a population by the total population size.**  

$$ P(+) = \frac{\#\ positive\ cases}{population\ size} $$  

**We know the probability of being positive and the probability of being negative must sum to 1.** 
  
$$ P(-) = 1 - P(+) $$  
  
**Probability of everybody at an event being negative for COVID-19 is the probability of one person being negative multiplied by the probability of every other person being negative. Or in more simple mathematical terms...**  
  
$$P(all\ -) = P(-)^{N}$$  

**The probability of at least one person being positive for COVID-19 and the probability of everybody at an event must add to 1.**

$$ P(at\ least\ one\ +) = 1 - P(all\ -) $$  
  
**The number of reported positive cases can be looked up using a reliable source such as covidactnow.org. However, the true number of positive cases will always be greater than the reported number of positive cases due to the presence of asymptomatic cases, lags in test reporting, and testing availability. We can account for this uncertainty by using a factor of safety. The factor of safety represents a multiple for how many more positive cases there are above and beyond the reported positive cases. For example, a factor of safety equal to 10 would mean that the true number of positive cases is 10x higher than the number of reported positive cases.**  
  
**As of the time of this writing it is estimated that a person infected with COVID has an incubation period of 7-14 days before experiencing any symptoms while still being contagious. In order to estimate the number of unknowingly positive people in a population, county level statistics for the length of the incubation period (we will use 10 days) can be used to estimate the number of positive people at a specific time within a population. This should give us a fairly accurate estimate of the prevalence of COVID at the county level.**  
  
$$ \#\ positive\ cases = FS * daily\ cases * incubation\ period$$  
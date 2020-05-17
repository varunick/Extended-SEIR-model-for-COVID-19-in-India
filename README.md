# Extended-SEIR-model-for-COVID-19-in-India
This is an extended SIER model to predict the death rate of coronavirus cases in India as of 17/05/2020.

The model uses the data for daily global deaths collated on "https://tinyurl.com/t59cgxn". Besides this, it also uses static data for age groups, probabilities, and ICU beds from UN Data.

The beds data has number of ICU beds per 100k population of many countries.

Age group data has total population of countries per age group.

Probabilities data has proability of people going from Infected to Critical and Critical to Dead per age groups.

This SIER model is an extension of the basic SIR (Susceptible infected recovered) epidemic model which uses differential equations for Susceptible, Exposed,Infected, Critical, Recovered and Dead population.

This model has assumed incubation period of COVID-19 as 9 days and number of days an infected person can infect other people as 3 days.it is also assumed that India is adding more ICU beds per day at a rate which is being calculated by the model. It also assumes that every critical patient who doesn't get an ICU bed dies. Also a recovered patient becomes immune to the virus (which looks like the actual scenario atleast till now)

India imposed complete lockdown on 22nd March. before this, the R_0 for India was close to 5. However during the lockdown, R_0 has averaged around 1.50. this model assumes that R_0 for India will remain at aorund 1.6 throughout this year even after lockdown is lifted and people follow the guidelines provided by the government. 

As of today 17/05, we have around 100-150 deaths per day in India.

After building this model, we can predict that around end of June/start of July, we will start seeing the deaths per day increasing exponentially. This will peak and go upto 12000 deaths per day around end of July and start of August. This is also the time when the number of patients requiring critical care will start to overwhelm the availability of ICU beds in India. However these numbers will then start coming down and return to current numbers like 100 deaths per day around start of September. So from this model we can predict coronavirus reaching its peak in India in June and July and then going down from Aug/Sep onwards.



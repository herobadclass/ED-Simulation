This discrete-event simulation model was created using SimPy to understand the impact of discharge times on ED wait times for impatient beds. 
For the purpose of this simulation, the ED patient journey starts after they have been admitted to a nursing unit for impatient care.

This project was done in collaborated with Providence Health Care, who provided three years of patient data.

Simulation summary:
- At the start of each hour a poisson distrubution is used to generate the number of patients admitted during the hour. The poisson distribution depends on the time of day and the day of week.
- Once patients are admitted, they will request a bed or wait until a bed is available.
- After a patient has seized a bed, their length of stay and discharge time is randomly chosen based on they day of week.
- The patient's bed is held for a hour after dischrage before returning to the pool of available beds.
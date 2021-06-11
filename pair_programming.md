# Pair Programming

* Create pairs for any paired assignment - Choose one person to be the “scheduler”
* Refer to your [Cohort Hub](README.md#quick-links) *Important Docs* Tab for pairs google sheet (this sheet is student facing)

### Example of simple code for random list of students, which can be used to choose pairs, groups of size k < n, and order of presentations: 

``` python
import numpy as np
RPP2_students = ['Becky_MDT', 'Bahar_PST', 'Andrew_EST', 'Mekdi_PST', 'Tony_PST', 'Robert_CT', 'Sean_PST', 'Nick_PST', 'Reza_CT', 'Bobby_AZ', 'Di_PST', 'Gary_EST', 'Matthew_EST', 'Shaheer_AZ', 'Marwah_PST']

np.random.choice(RPP2_students, replace=False, size=len(RPP2_students))
```
	
**Challenges**  
- Sometimes students may express that they don't want to work with another student. Different instructors handle this differently, 	posting the proposed pairs/groups to the team allows feedback and maybe adjustments.  
- Different time zones and work/family schedules can make pair programming difficult for part-time cohorts. 

	Ask instructor regarding:   
	- pairing based on time zones or schedules (alternatives to random pairings) 
	- due date extensions with prior approval

> [* updating pairs how to video](https://drive.google.com/file/d/1_2FXEfwQswyXi7L2QyT6RjbIrMmwbIkf/view?usp=sharing)
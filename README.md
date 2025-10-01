# 2025-Fall (semester 114-1)


## Final project timeline

- Pick up your project topic by `October 2nd` 
  -   [`Final project group list`](https://docs.google.com/spreadsheets/d/1RG6qqq0jFPrRBsApseZqcwsO5BIPCLq3vC9epwKlP5I/edit?usp=sharing)   
- Proposal presentation on `October 23rd`
- Final project report due on `December 18th`.

## Latex template [link](https://www.overleaf.com/project/5fb4c4325b0faa866d7218ed)  



<!--
(rescheduled from October 3rd due to class cancellation on the Typhoon day).
 (rescheduled from October 24th).
## Interactive feedback
- [Poll link](https://forms.gle/9G8ZT3BfhHmj4wnv6)
- [Response](https://docs.google.com/forms/d/1edoG4XJaAgARrq9S4artlCjaQW-f0nmntYyLhBfoi68/edit#responses)
-->





<!-- - In class of Sept. 29th, please fill out  [`Final Project Team Roster`](https://docs.google.com/spreadsheets/d/1RG6qqq0jFPrRBsApseZqcwsO5BIPCLq3vC9epwKlP5I/edit?usp=sharing)  -->

<!--  **Presentation order on Dec. 22: ['I', 'C', 'A', 'J', 'B', 'H', 'D', 'F', 'G', 'K', 'E']** -->


<!-- Presentation order on Oct. 20: ['F', 'A', 'E', 'C', 'D', 'B'] -->


<!--
```python
import random
groups = ['A','B','C','D','E','F','G','H','I','J','K']
#print (groups)
random.shuffle(groups)
print (groups)
```
-->




<!--  
# Midterm Statistics 

- $S_{scaled} = 100 \times\sqrt{\frac{S_{original}}{100}}$

- Average score = 86.40


- Standard deviation = 12.47
-->


<!--
import numpy as np

def generate_schedule(lst, previous_pairs=[]):
    if len(lst) < 2:
        return [[]]
    
    schedule = []
    
    if len(lst) % 2 == 1:
        for i in range(len(lst)):
            for result in generate_schedule(lst[:i] + lst[i + 1:], previous_pairs):
                schedule.append(result)
    else:
        a = lst[0]
        for i in range(1, len(lst)):
            pair = (a, lst[i])
            if pair not in previous_pairs and (pair[1], pair[0]) not in previous_pairs:
                new_previous_pairs = previous_pairs + [pair]
                for rest in generate_schedule(lst[1:i] + lst[i + 1:], new_previous_pairs):
                    schedule.append([pair] + rest)

    return schedule

def print_schedule(schedule):
    for round_num, round_pairs in enumerate(schedule, 1):
        print(f"\nRound {round_num}:")
        for pair_num, pair in enumerate(round_pairs, 1):
            print(f"\t Group {pair_num}: {pair}")

def find_pair_list(round_list):
    pair_a, pair_b, pair_c = round_list
    return pair_a, pair_b, pair_c

group_list = ["A", "B", "C", "D", "E", "F", "G", "H"]

schedule = generate_schedule(group_list)

for index in range(len(schedule)):
    round_list = schedule[index]
    index_temp = index
    for check_list in schedule[index+1:]:
        index_temp += 1 
        if any(pair in check_list for pair in round_list):
            replacement = [('x', 'x')] * len(schedule[0])
            schedule[index_temp] = replacement

schedule = [row for row in schedule if not all(pair == ('x', 'x') for pair in row)]
display(schedule)
print(" === Pairing up ===")
print_schedule(schedule)
-->

# OS Lab Quantum Widget Report
**Name:** ChomDevid
**Student ID:** IDTB110094
**Repository:** os-lab-quantum-IDTB110094

-----------------------------------------------------

## Level 2 — Audit Trails
### Observation Checkpoint 1

![Level 2 Output](image/level2.png)

----------------------------------------------

## Level 3 — The Exploit (TOC-TOU)
### Results from 5 runs
Run 1: 98
Run 2: 86  
Run 3: 84  
Run 4: 82  
Run 5: 80  

### Explanation
The inventory value changes with each run because the 
operating system decides unpredictably which of the 50 bots
gets CPU time first. If two bots read inventory.txt at the same
time before either writes their changes, one bot’s update can overwrite 
the other without any warning, causing some purchases to disappear. This is a
typical example of a time-of-check to time-of-use (TOC-TOU) race condition.
-----------------------------------

## Level 4 — The Patch (Mutex)
### Observation Checkpoint 3

![Level 4 Mutex](image/level4.png)

-----------------------------------

## Level 5 — Red Team vs Blue Team
### Observation Checkpoint 4

![Level 5 Result](image/level5.png)

--------------------------------------------------

## Level 6 — Secure Drop Zone
### Observation Checkpoint 5

![Level 6 Secure Zone](image/level6.png)

-----------------------------------------------------------------

## Level 7 — Forensic Cleanup
### Observation Checkpoint 7

![Level 7 Cleanup](image/level7.png)

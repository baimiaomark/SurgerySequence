# SurgerySequence

This folder includes 25 random test instances and corresponding solutions in "Surgery Sequencing Coordination with Recovery Resource Constraints"

##########
Please contact author Miao Bai for any question
###########

###########
Solution files: Solution1
#######
Includes performance of our proposed algorithm compared with MV, MV+SAA-GDR, NOPACU, NOPCU+SAA-GDR in terms of objective value and solution time in 25 test instances (Please refer to Table 3 in the manuscript for detail.
Columns:
1. Instance #,	
2. avg solution time of SH+SAA-GDR
3. average sequence time in SH+SAA-GDR
4. avg obj of SH+SAA-GDR
5. avg solution time of MV
6. avg obj of MV 
7. avg solution time of MV+SAA-GDR,	
8. avg obj of MV+SAA-GDR, 
9. avg solution time of NOPACU, 
10. avg obj of NOPACU, 
11. avg solution time of NOPACU+SAA-GDR,  
12. avg obj of NOPACU+SAA-GDR 

###########
Solution files: Solution2
#######
Includes performance of Heuristics in terms of objective value and solution time in 25 test instances (Please refer to Table 3 in the manuscript for detail). Each row cooresponds the performance of a heuristc in a specific instance
Columns
1. sequencing heuristic indicator: Random 0, SCF 1, LCF 2, HIHD 3, HDHI 4, MIX 5, Johnson 6, AlterJohnson 7, SVF 8,
2. JH hedging level indicator: mean 0, median 1, 65 percentile 2, 75 percentile 3
3. Instance #
4. average solution time of seq+JH (sequecing heuristic+job hedging heuristic)
5. average obj of seq+JH
6. average solution time of seq+SAA-GDR (sequecing heuristic+SAA-GDR)
7. average obj of seq+SAA-GDR


#######
Instance Files
########

Data structure (by rows)
Row 1.OR blocking cost ($/hour)

Row 2.Number of ORs

Row 3.Number of PACU beds

Row 4.Index of OR in the original OR pool (See Online Supplement EC.8 for the OR pool)

Row 5.Numer of scheduled surgeries in each OR 

Row 6-end: 
Each row includes distribution information of surgery duration and LOS in the PACU for a patient. Patients are listed in the sequence of their positions in ORs and their OR indices. That is, it follows the sequence of 1st patient in OR #1, 2nd patient in OR #1, ...., last patient in OR #1, first patient in OR #2, ....

Each row includes the following information in sequence: mean, standard deviation, lower bound and upper bound of surgery duration distribution (trancated lognormal distributions); followed by  mean, standard deviation, lower bound and upper bound of PACU LOS distribution (trancated lognormal distributions). 

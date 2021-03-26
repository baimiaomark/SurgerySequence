# SurgerySequence

This folder includes test 25 random test instances used in "Surgery Sequencing Coordination with Recovery Resource Constraints"

##########
Please contact author Miao Bai for any question
###########

Data structure (by rows)
Row1. OR blocking cost ($/hour)
Row2. Number of ORs
Row3. Number of PACU beds
Row4. Index of OR in the original OR pool (See Online Supplement EC.8 for the OR pool)
Row5. Numer of scheduled surgeries in each OR 
Row 6-end: 
Each row includes distribution information of surgery duration and LOS in the PACU for a patient. Patients are listed in the sequence of their positions in ORs and their OR indices. That is, it follows the sequence of 1st patient in OR #1, 2nd patient in OR #1, ...., last patient in OR #1, first patient in OR #2, ....

Each row includes the following information in sequence: mean, standard deviation, lower bound and upper bound of surgery duration distribution (trancated lognormal distributions); followed by  mean, standard deviation, lower bound and upper bound of PACU LOS distribution (trancated lognormal distributions). 

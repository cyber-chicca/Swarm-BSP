# Swarm-BSP
Reynolds Boids Swarm by Belief Space Planning dataset

This dataset is referred to the article: "Berman I, Zereik E, Kapitonov A, Bonsignorio F, Khassanov A,Oripova A, Lonshakov S and Bulatov V (2020) Trustable Environmental Monitoring by Means of Sensors Networks on Swarming Autonomous Marine Vessels and Distributed Ledger Technology. Front. Robot. AI 7:70. doi: 10.3389/frobt.2020.00070"

6 types of simulations have been performed (2 different noise values - w=0.5, w=0.9 - for each swarm of n=2, n=4, n=8 companion robots). For details check the above cited paper.

Each file name reports the experiment number (e.g. exp1), the additional noise (e.g. n09), the number of vehicles in the swarm (e.g. 8v) and the specific vehicle whose the log belongs to. Hence, file "exp1n098v_logVehicle1.txt" provides data logged by vehicle 1 during the first experiment with noise w=0.9 and a swarm made by 8 companions.

Each file contains the following variables, in the reported order:
- mgoal (3 values): 3D position and orientation to be reached (x-y-psi)
- m (3 values): planned 3D position and orientation of the vehicle (x-y-psi)
- err (3 values): error between desired and current vehicle position and orientation (x-y-psi)
- rplCnt (1 value): counter used when replanning occurs
- cmdTime (1 value): current time
- norm of SIGMA (1 value): norm of the BSP covariance matrix
- z (3 values): measure of the current 3D position and orientation of the vehicle (x-y-psi)
- noise (3 values): noise added to position/orientation measurements (x-y-psi)

For details about the meaning of the variable, please refer to the article above.

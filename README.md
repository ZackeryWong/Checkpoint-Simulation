# Checkpoint-Simulation
This is a checkpoint simulation using Anylogic

# Setup instruction:
1. Go to: https://www.anylogic.com/downloads/personal-learning-edition-download/
2. Fill in details to download
3. Run the downloaded file anylogic-ple-8.9.8.x86_64.exe to install Anylogic

# Engine version used: Anylogic 8.9.8 Personal Learning Edition

# Run Instruction
1. Go to folder SETUP 1/2
2. Run HTX_Simulation.alp
3. This will open up AnyLogic with the simulation loaded.
4. As our models for SETUP 1 and 2 are the same name, a popout will appear if you try to open it again. Click Ok to Close currently opened model.
5. Press the X on the Welcome Message.
6. Click on the Projects Pane > double on Main to open the simulation setup.
7. Press F5 or the Run button to run the simulation.

# How to Modify Simulation Parameters
To Change Traveller Spawn Rate
1.  Click on the pedSource block
2.  Look for Pedestrian in the properties window on the right
3.  Change the Arrival Rate

To Change hasBaggage Chance/ isLocal Chance
1. Click on the pedSource block
2. Look for Action in the properties window on the right
3. modify this block of code ped.hasBaggage = randomTrue(0.7); or ped.isLocal = randomTrue(0.5); 0.7 = 70% to be True

To change riskprofile/ docReady distribution
1. click on the distribution blocks named distDocReady / distRiskProfile
2. Look for Data in the properties window on the right
3. add/remove/change the data value and the weight

To change the chance for Referral
1. Look for pedSelectOutput node after psManual_PP and psAuto_PP.
2. Change the value for probability 1 to change the success probability
3. Change the value for probability 2 to change the fail probability

To Change Referral Process Success Rate
1. Look for ps_Referral node after goToReferral Node
2. Change the value for probability 1 to change the success probability
3. Change the value for probability 2 to change the fail probability

- To Change Simulation Run time
a. Under the projects Pane on the left, Click Simulation: Main with the X logo
b. This will open up a properties window on the right.
c. Look for Stop Time. Change this to the number of minutes you want the simulation to run for.

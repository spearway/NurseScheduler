# RosterDesNurses
# ===============

# Example of script that runs the executable with the list of arguments

bin/roster --sce datasets/n030w4/Sc-n030w4.txt --his datasets/n030w4/H0-n030w4-0.txt --week datasets/n030w4/WD-n030w4-1.txt --sol outfiles/solution.out

# Example of script to call the complete simulator of INRC-II

java -jar Simulator.jar --his testdatasets/n005w4/H0-n005w4-0.txt --sce testdatasets/n005w4/Sc-n005w4.txt --weeks testdatasets/n005w4/WD-n005w4-2.txt testdatasets/n005w4/WD-n005w4-0.txt testdatasets/n005w4/WD-n005w4-2.txt testdatasets/n005w4/WD-n005w4-1.txt --solver ./roster --runDir bin/ --outDir outfiles/ 

# Description of some notations that appear in the code/comment

- rotation: sequence of working days for a nurese. The shifts that are covered and the skils that are used can be different on each day. A rotation starts at the beginning of a week or after a resting day, and it ends at the end of a week or before a resting day. 
- break/pause/holiday/rest period: sequence of resting days. This period starts at the beginning of a week or after a working day, and it ends at the end of a week or before a working day. 
- stint: one rotation followed by a break

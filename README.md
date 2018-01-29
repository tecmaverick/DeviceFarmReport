# DeviceFarmReport

The script fecthes DeviceFarm test results and generates a JSON file. 

Pre-requisites:
1. AWS CLI installed and configured 

# Usage:
#Generates report for every tests in the project 
python main.py ReplaceWithProjectName

#Generates report for only the recent test in the project 
python main.py ReplaceWithProjectName -lastrun
python main.py ReplaceWithProjectName -lr



#Generates report for only the recent test in the project to the specific directory
python main.py ReplaceWithProjectName -lastrun --outputdirectory "path"
python main.py ReplaceWithProjectName -lr -od "path"


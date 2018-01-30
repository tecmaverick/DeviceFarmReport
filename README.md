# DeviceFarmReport

The script fetches DeviceFarm test results for a specific project and creates file in JSON format.

Pre-requisites:
1. AWS CLI installed and configured 

# Usage:
Generates report for every tests in the project 
```
python main.py ReplaceWithProjectName
```

Generates report for only the recent test in the project 
```
python main.py ReplaceWithProjectName --lastrun
python main.py ReplaceWithProjectName -lr
```

Generates report for only the recent test in the project to the specific directory
```
python main.py ReplaceWithProjectName -lastrun --outputdirectory "path"
python main.py ReplaceWithProjectName -lr -od "path"
```

For recent test run download artifacts including Screenshots, LOGS, Files etc
```
python main.py ReplaceWithProjectName --lastrun --downloadartifacts
python main.py ReplaceWithProjectName -lr -da
```

Download artifacts including Screenshots, LOGS, Files etc for all tests in the project
```
python main.py ReplaceWithProjectName --downloadartifacts
python main.py ReplaceWithProjectName -da
```

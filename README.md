# HEA-SMS
Detailed results of Hybrid Evolutionary Algorithm for the single machine scheduling problem with release dates and sequence dependent setups.<br>
### instances folder<br>
The folder includes 1800 instances.<br>
The explanation of a small example file is as follows:<br>
>5 2 -> number of jobs, number of machines(disregard)<br>
>0 -> disregard<br>
>0 -> disregard<br>
>1 3 4 222 -> job index, release date, processing time, due date(disregard)<br>
>2 2 3 1593<br>
>3 8 3 685<br>
>4 5 8 966<br>
>5 7 5 113<br>
>6 2 5 9 3-> initial setups<br>
>0 3 7 5 3 -> setup from job 1(row) to job n(column) (disregard diagonal)<br>
>3 0 2 8 7<br>
>2 4 0 5 6<br>
>4 3 5 0 2<br>
>6 7 3 5 0 -> setup from job 5(row) to job n(column) (disregard diagonal)
### HEA-RESULT.csv<br>
This file contains the best and average makespan values obtained by the HEA algorithm for various test instances.
### SOLUTION.XLSX<br>
This file contains the best solutions obtained by the HEA algorithm for various test instances.
### Executable file
When executing, use the following command: ./hea runconfig25.json
The param1 file provides all the parameter configurations required for running instances of all scales.
The runconfig25.json file specifies some runtime parameter settings. The instancefile should be organized according to the instance scale. If you change the instance scale, please update both the "instanceFile" and the "paramName" accordingly, because at runtime, the program will load different parameters based on the "paramName".The instance files are located in the "instance" folder, and the result files are stored in the "result" folder. Before running, please ensure that both folders exist.

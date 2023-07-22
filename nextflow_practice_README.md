# Nextflow_Practice
## We are working with nextflow DSL2 as its the updated version
### Most of the examples are borrowed from youtube tutorials and then modfifed to play around with it.
Documentation of my nextflow learning journey
- any file with .nf extension is a nextflow file.

### 1st nextflow script- This is the replication of a very basic youtube tutorial on nextflow- [Youtube tutorial link]( https://www.youtube.com/watch?v=sp45Bzri2sA)
- In this example- our file is [hellopython.nf](https://github.com/snehacodes15/nextflow_practice/blob/main/hellopython.nf)

## Description of the contents inside the hellopython.nf file-
- Contents

![image](https://github.com/snehacodes15/nextflow_practice/assets/129862776/590da0b5-82d7-49a3-a803-161606d30ef8)

  
  1. The name of the file is hellopython.nf, where nf is extension for nextflow file.
  2. process refers to a task/program/script that can be executed
  3. sayhello refers to the name of the process. (Think of it in a similar fashion where we name a function in python)
  4. { and the """ are part of nextflow syntax
  5. In nextflow, process script is executed as a bash script by deafult. However it supports other languages too. Inside our nextflow script, we are trying to execute a process in python. Hence we need to add the shebang line to indicate that its apython script - #!/usr/bin/python3
  6. For the user to know what is the path of their python interpreter, type "which python" in the terminal, which will display the path to thier python inyterpreter and accordingly add that line after the shebang in the script.
  7. workflow mentions which process to execute. Here we want to execute sayhello process.
  8. To run this file- type- nextflow run hellopython.nf -process.echo
  9. we have to add process.echo since we want to display "hello world" on the terminal. To display anhything on the terminal instead of lrinting to a file, we need to add -process.echo command while running the nextflow syntax.

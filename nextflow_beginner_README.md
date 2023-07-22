# Nextflow_Practice
## We are working with nextflow DSL2 as its the updated version
### Most of the examples are borrowed from youtube tutorials and then modfifed to play around with it.
Documentation of my nextflow learning journey
- any file with .nf extension is a nextflow file.
- In this example- our file is [hellopython.nf](https://github.com/snehacodes15/nextflow_practice/blob/main/hellopython.nf)

## Description of the contents inside the hellopython.nf file-
- Contents
<br/> process sayHello {
    
"""
#!/usr/bin/python3

print("hello world")

"""

}

workflow {
    sayHello()
    }

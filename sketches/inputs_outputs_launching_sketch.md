# File storage

### Input files

All input files will be stored in __./inputGraphs__ directory

### Output files

Output files will be stored in __./outputResults__ directory

There will be subdir:
- __allPathsPrinted__ - for storing results with all paths printed


---

# Launching

## Launching command:
```
python ACOShortestPath_Run.py input_filename vertex_start vertex_end pheromone_influence desirability_influence evaporation_coefficent iters_num runs_num print_all_paths[y/n]
```
---

# Input files

Input graph files should look like this:

```
vertexesNum = x
edgesNum = y
1. vertex_start vertex_end weight
2. vertex_start vertex_end weight
...
y. vertex_start vertex_end weight
```
---

# Output files

### Output filenames

Output files will be named: `inputFilename_launchTimeAndDate_parameters`

`parameters`:
- vertex_start
- vertex_end
- pheromone_influence
- desirability_influence
- evaporation_coefficent
- iters_num

### Output files

```
------------------------------------
Run:          run_number
Input:        inputFilename
Parameters:
    - vertex_start =            sth
    - vertex_end =              sth
    - pheromone_influence =     sth
    - desirability_influence =  sth
    - evaporation_coefficent =  sth
    - iters_num  =              sth
Start:        timeAndDate
End:          timeAndDate
Time running: time

Shortest path:
weight =      pathWeight
v1 - v2 - ... - vn

All paths:[optional]
1. v1 - v2 ...
2. v1 - v2 ...
...
k. v1 - v2 ...
------------------------------------
```

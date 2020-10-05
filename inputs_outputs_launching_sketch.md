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
python ACOShortestPath_Run.py input_filename vertex_start vertex_end pheromone_influence edge_desirability evaporation_coefficent iters_num runs_num print_all_paths[y/n]
```
---

# Input files format

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

# Output files format

### Output filenames

Output files will be named: `inputFilename_launchTimeAndDate_parameters`

`parameters`:
- vertex_start
- vertex_end
- pheromone_influence
- edge_desirability
- evaporation_coefficent
- iters_num

### Output files

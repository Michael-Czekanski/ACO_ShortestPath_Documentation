# Launching args

```
if len(args) != 10:
  print("Invalid number of arguments.")
  exit
```

# Reading from inputs

- New class: `ACOShortestPathInputReader`
  -

# Creating and writing to outputs

# Run file pseudocode

```
launchingTimeAndDate = currentTimeAndDate
read args
read graph from input file
for i = 0; i < runs_num:

  if print_all_paths:
    redirect all prints to -> programData/allPathsTemp file


  shortestPath = findShortestPath()

  if print_all_paths:
    stop redirecting all prints to -> programData/allPathsTemp file



```

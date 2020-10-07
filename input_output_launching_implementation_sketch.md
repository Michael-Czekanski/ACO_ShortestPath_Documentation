# Launching args

```
if len(args) != 10:
  print("Invalid number of arguments.")
  exit
```

# Reading from inputs

New class: `ACOShortestPathInputReader`
Methods:
- readGraphFromInputFile(filename)

# Creating and writing to outputs

New class:      `ACOShortestPathOutputWriter`

Methods:
- writeOutputToFile(data:[ACOShortestPathOutputData])
- createOutputFile(launchingTimeAndDate, inputFilename, vertex_start, vertex_end, pheromone_influence, desirability_influence, evaporation_coefficent, iters_num) -> [File]

New structure:  `ACOShortestPathOutputData`

Methods:
- ctor(run_number, inputFilename, vertex_start, vertex_end, pheromone_influence, desirability_influence, evaporation_coefficent, iters_num, algorithm_start_time, algorithm_end_time, elapsed_time, path:[Path], print_all_paths:[bool])


# Run file pseudocode

```
launchingTimeAndDate = currentTimeAndDate()
read args
inputGraph = ACOShortestPathInputReader.readGraphFromInputFile(...)
outputFilename = ACOShortestPathOutputWriter.createOutputFilename(...)
for i = 1; i <= runs_num:

  if print_all_paths:
    redirect all prints to -> programData/allPathsTemp file

  startTime = currentTimeAndDate()

  shortestPath = findShortestPath()

  endTime = currentTimeAndDate()
  elapsedTime = endTime - startTime

  if print_all_paths:
    stop redirecting all prints to -> programData/allPathsTemp file

  data = ACOShortestPathOutputData(certainArguments)
  ACOShortestPathOutputWriter.writeOutputToFile(data)



```

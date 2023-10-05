<h1 align="center" id="title">Genetic Algorithm</h1>

<p id="description"><b>Y = w1x1 + w2x2 + w3x3 The equation has 3 inputs (x1 to x3) and 3 weights (w1 to w3) as shown and inputs values are (x1x2x3)=(4-27). The goal is to identify the parameter values (weights) that optimize the given equation. Ideally a tuple of weights with a combination of positive-negative-positive values would be the solution. To achieve this a Genetic Algorithm (GA) can be employed to search for the optimal values that maximize the equation.</b></p>
<p id="Explaination">In the initial phase, a population comprising 50 tuples is generated, each tuple consisting of three randomly assigned values falling within the range of -10 to 10. Subsequently, the fitness function, denoted as "fitness()," is employed to compute a fitness score for each member of this population. The fitness score is calculated based on the equation w1 * x1 + w2 * x2 + w3 * x3, where the values of x1, x2, and x3 are fixed at 4, -2, and 7, respectively.

Upon reaching the first generation, the fitness function specifically selects tuples with a characteristic structure: positive, negative, positive. This structural preference is attributed to the fact that such tuples yield the most favorable fitness scores. Among the original population, a subset of 10 parent nodes is chosen, and these parent nodes serve as the basis for generating offspring.

The mechanism employed for generating offspring includes single-point crossover and a mutation rate of 10%. As the algorithm progresses through subsequent generations, the program ensures that the structural pattern of positive, negative, positive values within each tuple is maintained. However, the program actively seeks to enhance the fitness scores by progressively increasing the weights.

In scenarios where the entire initial population consists of exclusively positive values, an intriguing observation emerges. Specifically, during subsequent generations, the second value within each tuple approaches zero and eventually becomes negligible or zero. This phenomenon can be attributed to the cumulative effect of the 10% mutation rate, which predominantly results in minimal changes due to the proximity of the value to zero. Consequently, the second value remains constant throughout subsequent generations.

Conversely, when the initial population comprises solely negative values, a different pattern emerges. In this case, the first and third values within each tuple gradually converge to zero. Meanwhile, the second value consistently diminishes with each passing generation. This behavior is a consequence of the mutation process steadily reducing the magnitude of these values over time.</p>
<p>Hence, it can be inferred that the algorithm, through the utilization of the fitness function, acquires a clear understanding of the optimal configuration for the equation's values right from the commencement of the algorithm.</p>
  
  
<h2>🧐 Features</h2>

Here're some of the project's best features:

*   Python
*   Genetic Algorithm
# Instructors Allocation Algorithm using Maximum Flow
This repository contains an algorithm for allocating instructors to courses. It utilizes maximum flow algorithms in networks to solve the allocation problem. The solution's description can be found [here](https://drive.google.com/file/d/1QXTqFaD0hu9iJ6eI2EZQ1UUdWFIuJNfu/view?usp=sharing).

## Algorithm Versions
The repository includes two versions of the algorithm:

1. Restricted Version: This version does not take into account a preference scale and only considers the possibility of allocating an instructor to a course. It is based on the implementation of the Edmonds-Karp algorithm.
1. General Version: This version considers a preference scale, allowing instructors to prioritize certain courses over others. It is based on the implementation of a minimum-cost maximum flow algorithm.

## Getting Started

To run the algorithm, follow these steps:

1. Clone the repository:

   ```
   git clone https://github.com/Joao03Guilherme/instr-aloc
   ```

2. Navigate to the `Algoritmo_Geral` folder.

3. Prepare the input data by updating the following two CSV files:

   - `data.csv`: This file contains the input data for instructors. Each row represents an instructor and includes the following columns: "email," "interest," "name," and "possible_months" (this column can be omitted).

   - `course_data.csv`: This file contains data related to the staffing requirements for each course. It consists of three columns: "course," "min_staff," and "max_staff."

4. Execute the `instr_aloc_flow.py` file to run the algorithm.

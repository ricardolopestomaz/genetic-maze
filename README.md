# Genetic Maze

![Status](https://img.shields.io/badge/status-completed-brightgreen)

A C project implementing a **Genetic Algorithm** for maze navigation, where individuals evolve to find the optimal path to the exit.

---

## 📌 About the Project

This project uses evolutionary computation techniques to solve maze navigation problems. Each individual has a chromosome encoding movements on the map, and evolution occurs through selection, crossover, and mutation.

---

### Best Individual per Generation
<p align="center">
  <img src="https://i.ibb.co/pBLMVMRZ/Captura-de-tela-2025-06-25-101349.png" alt="Project Example">
</p>
<p align="center">
  <img src="https://i.ibb.co/2Ytx8D1S/AEF52-A28-7742-40-B9-BD06-419-DDA63-D509.png" alt="Project Example">
</p>

---

## ⚙️ Features

- Individual represented by a chromosome containing movements:  
  - `U` - Up  
  - `D` - Down  
  - `L` - Left  
  - `R` - Right
- Simulation of the path in the maze considering collisions and map boundaries.
- Control of visible movements from the starting position via a queue of valid moves.
- Full Genetic Algorithm: selection, crossover, mutation, and population evolution.
- Fitness evaluation based on distance to the exit, steps taken, and success.
- Generation of graphs and reports for analyzing results.

---

## 🧩 Code Structure

- `individual.c/h` - Creation, initialization, and freeing of individuals.
- `simulation.c/h` - Simulation of individuals' movements in the maze.
- `population.c/h` - Population management and fitness-based sorting.
- `crossover.c/h` - Chromosome crossover operations.
- `mutation.c/h` - Chromosome mutation functions.
- `fitness.c/h` - Calculation of individuals' fitness.
- `map.c/h` - Maze representation and manipulation.
- `logs.c/h` - Simulation logs and reports.
- `graphs/` - Graph generation for result analysis.

---

## 🚀 How to Run

1. Clone the repository:
    ```bash
    git clone https://github.com/ricardolopestomaz/labirinto-genetico.git
    cd labirinto-genetico
    ```
2. Compile the project:
    ```bash
    gcc main.c _crossover/crossover.c _fitness/fitness.c _individuo/individuo.c _mapa/mapa.c _mutacao/mutacao.c _populacao/populacao.c _props/props.c _selecao/selecao.c _simulacao/simulacao.c _logs/logs.c graficos/graficos.c -o main.exe
    ```
3. Run the program:
    ```bash
    ./main.exe
    ```

---

## 📧 Contact

Ricardo Lopes Tomaz
📧 ricardolptz42@gmail.com  
[LinkedIn](https://www.linkedin.com/in/ricardo-lopes-tomaz-19053b297?originalSubdomain=br)

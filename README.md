# 📦 Genetic Algorithm for the Bin Packing Problem

## 📌 Description
This project implements a **Genetic Algorithm in C** to solve the **Bin Packing Problem**, a classical NP-hard optimization problem.  
The goal is to assign objects to boxes while minimizing the number of boxes used and respecting capacity constraints.

---

## 🧠 Problem Definition
- Each object has a specific size
- Each box has a fixed maximum capacity
- Objects must be assigned to boxes
- The total size of objects in a box cannot exceed its capacity
- The objective is to **minimize the number of boxes**

---

## ⚙️ Algorithm
The genetic algorithm includes:
- Random generation of valid initial solutions
- Fitness evaluation based on the number of boxes used
- Tournament selection
- One-point crossover
- Random mutation
- Iterative evolution over multiple generations
- Continuous improvement of the best solution found

---

## 🏗️ Implementation Overview
- `solu_t` : Represents a candidate solution (chromosome)
- `pop_t` : Represents a population of solutions
- `Algo_genetique()` : Main genetic algorithm loop
- `selectionner()` : Selection operator
- `croisement()` : Crossover operator
- `mutation()` : Mutation operator
- `ind_validite()` : Fitness and feasibility check
- `lire_fichier()` : Reads problem parameters from a file

---

## 📄 Input File
The program reads its parameters from `projet_param.txt`.


### Example:
 - B: 10
 - n: 5
 - T: 2 3 4 1 5

Where:
- `B` is the box capacity
- `n` is the number of objects
- `T` contains the object sizes

---

## ▶️ Compile and Run
```bash
gcc main.c -o genetic_bin_packing
./genetic_bin_packing


# 🎲 Snakes and Ladders — Statistical Simulation and Probability Analysis in R

A modeling and simulation project of the *Snakes and Ladders* game developed in R, focused on logical validation, statistical analysis, and insight generation from simulated data.

---

## Overview

This project aims to analyze the behavior of the Snakes and Ladders game under different scenarios using computational simulation to estimate probabilities, averages, and structural patterns.

The approach combines mathematical modeling, rule validation, and exploratory analysis to answer relevant questions about game dynamics, randomness, and balance.

---

## Objectives

* Model the game programmatically in R
* Validate the consistency of the implemented rules
* Simulate thousands of games for statistical analysis
* Evaluate the impact of rule modifications
* Identify patterns and generate actionable insights

---

## Project Structure

```text
snakes-ladders/
│
├── slides.qmd              # Final presentation (Quarto / RevealJS)
├── R/
│   ├── board.R             # Board structure (snakes and ladders)
│   └── simulate.R          # Simulation functions
│
├── figs/                   # Charts and images
├── output/                 # Rendered files
└── README.md
```

---

## Problem Modeling

The board was represented as a transition system between squares:

* Ladders: move the player forward
* Snakes: move the player backward
* Winning rule: reach or exceed the final square

All logic was encapsulated in reusable functions, enabling efficient simulation of multiple scenarios.

---

## Methodology

The project was structured into four main stages:

1. Board modeling
2. Rule validation
3. Game simulation (Monte Carlo)
4. Statistical analysis of results

Thousands of simulations were performed for each scenario to ensure statistical stability and reliability.

---

## Validation Procedures

Before conducting the final analysis, several validation checks were performed to ensure model reliability:

* Uniform dice distribution
* Correct application of snakes and ladders after movement
* Proper turn alternation between players
* Edge case handling

  * Victory when reaching or exceeding the final square
  * Prevention of invalid states
  * Infinite loop control

---

## Research Questions

### Q1. Does the First Player Have an Advantage?

The simulation indicated that the player who starts the game has a slight statistical advantage, with a win probability above 50%.

---

### Q2. How Frequent Are Snakes and Ladders?

Occurrences of snakes and ladders are frequent throughout the games, demonstrating that these elements play a structural role in the game's behavior.

---

### Q3. What Is the Impact of Probabilistic Ladders (50% Effectiveness)?

When ladder effectiveness was reduced, the following effects were observed:

* Increase in the average number of turns
* Greater variability in game duration

These findings highlight the role of ladders as a game-acceleration mechanism.

---

### Q4. How Can the Game Be Made More Balanced?

A two-phase search procedure was conducted to identify the optimal starting position for Player 2 that would bring both players' win probabilities closer to 50%.

Small adjustments to the initial conditions were sufficient to neutralize the first-player advantage.

---

### Q5. What Is the Impact of Immunity to the First Snake?

Allowing Player 2 to ignore the first snake encountered altered the win probabilities, demonstrating the game's sensitivity to rule changes.

---

## Key Insights

* There is a structural advantage for the starting player.
* Game duration remains relatively stable despite randomness.
* Snakes and ladders directly influence game dynamics and variability.
* Reducing ladder effectiveness significantly increases game length.
* Small rule changes can substantially affect game balance.

---

## Technologies Used

* R
* RStudio
* Quarto (RevealJS)
* tidyverse
* ggplot2
* knitr
* kableExtra

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/ThaynanRodrigues/Snakes-Ladders.git
cd Snakes-Ladders
```

### 2. Open the Project in RStudio

### 3. Render the Presentation

```bash
quarto render slides.qmd
```

---

## Presentation

The project includes a presentation developed in Quarto, focusing on:

* Methodological clarity
* Logical validation
* Data visualization
* Insight communication

---

## Author

**Thaynan Rodrigues**
**Data Analyst | Data Scientist**

---

## Contact

* [LinkedIn](https://www.linkedin.com/in/thaynanrodrigues/)
* [GitHub](https://github.com/ThaynanRodrigues)

# Decodelabs-Task-1-AryanT
Designed Number Guessing Game using Java
# Project 1: The Number Game
### DecodeLabs Engineering Directive // Phase 1: Logic & Control Flow

Welcome to the team! Project 1 serves as your foundational logic phase as a Java Developer at DecodeLabs. Before advancing to enterprise-level applications, this project requires you to master managing program state, control flow, and real-time user input handling.

---

## 📌 Project Overview & Objectives

The goal of this project is to bridge intuition and machine randomness by engineering a *Random Logic Engine*. You will build a dynamic, looping command-line program that interacts with a user to guess a hidden, programmatically generated number.

* *Mission:* Generate a stochastic number within a specified range ($1 \text{ to } 100$) and sustain a active feedback loop until the logical termination state is met.
* *Core Focus:* Transitioning away from simple arithmetic and mastering program state management, looping control constructs, and user interaction streams.

---

## 🛠️ Key Concepts & Toolkit

To meet the quality verification standards, your implementation must utilize the following architectural tools:

### 1. Stochastic Generation (java.util.Random)
To ensure optimal object flexibility, you must use java.util.Random instead of Math.random(). 
* *The Zero-Index Shift:* Computer logic operates on a $0$-indexed system where random.nextInt(100) returns a value from $0 \text{ to } 99$. 
* To shift this to human logic ($1$-indexed range of $1 \text{ to } 100$), your logic engine must apply an offset:
    java
    int targetNumber = random.nextInt(100) + 1;
    

### 2. Stream Capture (java.util.Scanner)
The program must instantiate a java.util.Scanner to act as a listening device for System.in. This tokenizes the raw incoming byte stream into type-safe integers via scanner.nextInt().

### 3. Logic Architecture (Feedback Loop)
The application state must be governed by a conditional execution path that evaluates user choices against the hidden memory state

## 📋 Requirements Checklist

### Mandatory Criteria (Qualification Criteria)
Your project must satisfy all baseline specifications to unlock subsequent industrial training kits:
- [ ] *Stochastic Generation:* Automatically generate a random target number between 1 and 100.
- [ ] *Stream Capture:* Accept and process numerical user guesses natively from the console.
- [ ] *Instant Feedback Loop:* Print "Too High" if the guess exceeds the target, or "Too Low" if it falls short.
- [ ] *Termination State:* End execution cleanly with a success message once the correct number is identified.
- [ ] *Engine Persistence:* Sustain a continuous 'live' execution loop until the logical win condition is satisfied.

### Optional Enhancements
To maximize your quality evaluation profile, consider implementing the following expansion vectors:
- [ ] *Attempt Restrictions:* Enforce a strict upper bound limit on the number of attempts permitted per game.
- [ ] *Multi-Round Engagements:* Prompt the user to clear multiple consecutive rounds without exiting the process context.
- [ ] *Scoreboard System:* Compute and display a final performance score based on metrics like efficiency and fewer attempts.

---

## 🚀 Getting Started

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- Any standard IDE or terminal environment

### Execution
1. Clone your assigned team repository.
2. Compile the logic engine core:
   ```bash
   javac NumberGame.java
   1. Boot up the runtime application: 
   ```bash
java NumberGame

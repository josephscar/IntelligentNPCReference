# IntelligentNPCReference

**Prebuilt AI NPCs in different AI styles.**  
A reference project for building **intelligent, explainable NPC behavior** in Unity games.

---

## Overview

**IntelligentNPCReference** is a single Unity project containing **multiple scenes**, each showcasing a different AI decision-making architecture under the **same gameplay conditions**.

The project is designed as:
- A **learning tool** for understanding game AI patterns
- A **reference implementation** for future Unity projects

All AI styles operate within the same **simple shooter arena**, allowing direct comparison of behavior, adaptability, and complexity.

---

## Core Design Principles

- **One game, multiple AI brains**
- Shared systems across all scenes:
  - Navigation (NavMesh)
  - Perception (vision, line-of-sight)
  - Combat (health, damage, cooldowns)
  - World context (targets, memory)
- Only the **decision-making logic changes per scene**

This ensures fair, apples-to-apples comparison between AI styles.

---

## Implemented AI Styles

### 🟢 Finite State Machine (FSM)

A classic AI architecture where NPCs operate in **one state at a time** (e.g., Idle, Chase, Attack, Retreat).  
State transitions occur when predefined conditions are met.

- Establishes the behavioral baseline
- Highlights predictability and simplicity
- Demonstrates limitations as complexity grows

---

### 🟡 Behavior Tree (BT)

A hierarchical decision system composed of **selectors, sequences, conditions, and actions**.  
The tree is evaluated every frame to determine the highest-priority valid behavior.

- Shows structured, modular decision logic
- Demonstrates scalability compared to FSMs
- Reflects industry-standard NPC architecture

---

### 🔵 Utility AI

A score-based decision system where each possible action is evaluated using **continuous utility functions**.  
The highest-scoring action is chosen dynamically at runtime.

- Produces smooth, adaptive, non-binary behavior
- Integrates naturally with stat- and modifier-driven systems
- Serves as the project’s flagship AI implementation

---

### 🟣 Goal-Oriented Action Planning (GOAP)

A planning-based AI system where NPCs pursue **high-level goals** by dynamically constructing action sequences based on world state and action costs.

- Demonstrates deliberative, long-term reasoning
- Enables emergent behavior without hardcoding sequences
- Highlights trade-offs between intelligence and computational cost

---

### 🔴 Machine Learning (ML-Agents) *(Optional / Advanced)*

A reinforcement-learning-based AI trained through rewards and penalties rather than explicit rules.

- Serves as a contrast to handcrafted AI
- Demonstrates ML integration within Unity
- Highlights challenges of explainability and control

---

## Why This Project Exists

- Learning and experimentation
- AI system prototyping
- Technical interviews and portfolio review
- Reference for future Unity projects requiring intelligent NPCs

---


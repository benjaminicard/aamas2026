
# Moral Evaluation of Speech Acts — Truthfulness, Lies and Ethical Dilemmas — Modeled and Implemented with ASP

This repository accompanies our paper submission to [AIES 2025](https://www.aies-conference.com/2025/). 

It provides a Python-based implementation of an Answer Set Programming (ASP) framework for modeling and evaluating speech act utterances in high-stakes ethical scenarios. Using Sartre’s The Wall (1939), the framework integrates key moral theories—deontologism, principialism, and consequentialism—to assess the permissibility of speech acts based on speakers' intentions, truth-values of their utterances, moral motives, and outcomes for third parties.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Code Structure](#code-structure)

## Overview

Ethical dilemmas often extend beyond physical actions to include verbal actions, such as lying, truth-telling, and withholding information. This project provides a systematic ASP-based framework for analyzing the ethical dimensions of speech acts, focusing on:

1. **Intentions:** Whether the speaker is honest or dishonest.
2. **Truthfulness:** The objective accuracy of the statement.
3. **Motives:** Benevolent or malevolent goals.
4. **Outcomes:** Beneficial or detrimental consequences.

The case study examines Jean-Paul Sartre’s *The Wall*, a story set during the Spanish Civil War. The narrative vividly illustrates the ethical complexity of lies, distinguishing between falsehoods and truthful lies with unintended, harmful consequences. The protagonist, Pablo Ibbieta, lies twice during an interrogation to protect his comrade Ramon Gris. In his first lie, Pablo provides false information that accidentally saves Ramon’s life. In his second lie, he unwittingly tells the truth, leading to Ramon’s death. These contrasting outcomes demonstrate how intentions, motives, and consequences intersect in speech acts, making Sartre’s story an ideal context for analysis.

## Features

- **ASP Integration:** A logic-based approach using Clingo and Clyngor for modeling and reasoning.
- **Ethical Theories:** Comprehensive implementation of deontologism, principialism (with two variants), and consequentialism (with immediate and cumulative utility).
- **Speech Act Taxonomy:** Classifies utterances as objective truths, erroneous truths, objective lies, or erroneous lies.
- **Utility Calculations:** Models the ethical impact of actions using expected and real outcomes.
- **Dynamic Scenarios:** Handles epistemic and moral considerations in evolving contexts.

## Installation

### Prerequisites

- Python 3.8 or higher
- `pip` package manager

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/aies2025-asp.git
   cd aies2025-asp
   ```

2. Install dependencies:
   ```bash
   pip install clingo
   pip install clyngor-with-clingo
   ```

## Usage

1. Define the ethical dilemma in the provided ASP framework.
2. Run the main script:
   ```bash
   python aies2025_asp_clingor.py
   ```
3. Review the output, which includes computed answer sets and evaluations for each moral theory.

### Example Output

The script evaluates Pablo Ibbieta’s speech acts under different ethical theories, showing:
- Permissibility of objective lies and erroneous lies based on moral theories.
- Utility-based rankings for consequentialism.
- Decision-making exceptions in principialism.

## Code Structure

- `aies2025_asp_clingor.py`: Main script integrating both programs for ethical evaluation.
- **Program 1:** Implements deontologism and principialism1, focusing on absolute duties and principled exceptions.
- **Program 2:** Extends the framework to principialism2, consequentialism1, and consequentialism2, incorporating counterfactual reasoning and utility calculations.

### Key Components

1. **Agents and Situations:** Models interactions and beliefs of agents like Pablo, Ramon, and the Falangists.
2. **Ethical Theories:** Implements deontologism, principialism, and consequentialism with structured rules.
3. **Answer Set Reasoning:** Uses Clingo and Clyngor for computational logic and ethical assessment.



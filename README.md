# Modular Quiz Application (Python OOP)

An interactive command-line quiz application built using Python and Object-Oriented Programming (OOP) principles. 
The project demonstrates clean software architecture by separating data structures, data models, and game control logic into independent modules.

## Features
* **Modular Architecture:** Decouples game content (`data.py`) and object models (`question_model.py`) from the runtime brain (`quiz_brain.py`).
* **Object-Oriented Design:** Transforms raw dictionary data into structured, reusable object entities.
* **Case-Insensitive Validation:** Automatically normalizes inputs so guesses are verified correctly regardless of capitalization (e.g., "true", "True", or "TRUE").
* **Real-Time Score Tracking:** Keeps active record counts of current scores and progress milestones after every single answer.

## System Architecture & File Structure
* `main.py`: The entry point that orchestrates object creation, compiles the question bank, and handles the primary execution loop.
* `question_model.py`: Defines the foundational blueprint for a single `Question` entity.
* `quiz_brain.py`: Contains the core `QuizBrain` class responsible for guiding loops, prompting inputs, and aggregating analytics scores.
* `data.py`: Acts as the local storage text database holding raw question dictionaries.

## Technical Concepts Used
* **Dependency Injection & Composition:** Passes an compiled array buffer of unique `Question` objects straight into the `QuizBrain` instance wrapper.
* **Encapsulation:** Seals index pointers and running scores entirely inside instance scopes via the `self` keyword.
* **Dynamic Evaluation Loops:** Binds a runtime execution loop directly to class inquiries (`still_has_question`) for self-governing code lifecycles.
* **Case-Insensitive String Methods:** Employs `.lower()` normalization chains to avoid processing failures during validation steps.

## Preview Example
```text
Q.1: A slug's blood is green. (True/False): true
You got it right
The correct answer was: True
Your current score is: 1 / 1


Q.2: The loudest sound produced by any animal is 188 decibels. (True/False): false
That's wrong
The correct answer was: True
Your current score is: 1 / 2


You've completed the quiz.
Your final score was: 1/2
```

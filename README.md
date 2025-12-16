# silk-road-robots-simulator
Java-based simulator for the “Silk Road… with Robots!” problem, developed as an academic project using object-oriented design and visual simulation.

# 🧾 README –Silk Road … with Robots! (Final Project Closure)

## 1. Overview

Cycle 5 represents the **final development stage** of the *Silk Road… with Robots!* simulator. During this phase, all functionalities developed in previous cycles were fully integrated, resulting in a **stable, modular, and visually consistent final product**.

The project was consolidated and executed entirely in **BlueJ**, including all functional classes and testing modules. A final review of the architecture, behavior, and documentation was conducted to ensure clarity, maintainability, and correctness.

The main objective of this cycle was to deliver a **fully functional, readable, and interactive simulator** capable of visually representing and solving the *The Silk Road… with Robots!* problem.

---

## 2. Cycle Objectives

- Integrate all modules (`SilkRoad`, `Robot`, `Store`, `Spiral`, `SilkRoadContest`) into a coherent and functional system.
- Execute unit, collective, and acceptance tests to ensure system correctness.
- Review and refine the final architecture, ensuring proper communication between classes.
- Provide clear documentation based on the final implementation.
- Present the complete simulation, validating both logical behavior and visual feedback.

---

## 3. Project Structure

The project is composed of the following main modules:

- **SilkRoad.java**  
  Main simulation controller. Manages robots, stores, profits, visualization, and robot movement.

- **Store.java**  
  Defines different store types (`normal`, `autonomous`, `fighter`, `trap`) and manages their money and visual state.

- **Robot.java**  
  Represents robots (`normal`, `neverback`, `tender`, `dummy`) with individual behavior and profit tracking.

- **Spiral.java**  
  Calculates `(x, y)` coordinates to position elements along a spiral layout on the visual board.

- **SilkRoadContest.java**  
  Handles contest logic and marathon problem resolution (`solve` and `simulate` methods).

- **SilkRoadException.java**  
  Custom exception handling for simulator-specific errors.

- **shapes (Canvas, Rectangle, Circle)**  
  Visual library used to render robots, stores, profit bars, and animations.

### Testing Classes
- **SilkRoadC4Test / SilkRoadCC4Test** – Unit and collective tests.
- **SilkRoadContestTest / SilkRoadContestCTest** – Contest-specific tests.
- **SilkRoadATest** – Acceptance tests with visual verification and user interaction.

---

## 4. Fulfilled Requirements

### 🔧 Functional Requirements
- Creation of a Silk Road with variable length.
- Addition and removal of robots and stores at valid positions.
- Implementation of specialized store and robot types with custom rules:
  - **Autonomous stores** place themselves automatically.
  - **Fighter stores** only reward robots with higher accumulated profit.
  - **Trap stores** cause visiting robots to lose money.
  - **Neverback robots** cannot move backwards.
  - **Tender robots** collect only half of the available money.
- Global store resupply (`resupplyStores()`).
- Full simulation reset (`reboot()`).
- State queries (`emptiedStores()`, `profitPerMove()`).
- Complete visual control:
  - Stores, robots, profit bar.
  - Blinking effect for the robot with the highest profit.

---

### 🧱 Design Requirements
- Modular architecture using core classes (`SilkRoad`, `Robot`, `Store`, `Spiral`).
- Clear separation of responsibilities:
  - **Logic:** `SilkRoad`
  - **Models:** `Store`, `Robot`
  - **Visualization:** `Spiral` + `shapes`
- Fully integrated class diagram (BlueJ structure).
- Code refactoring to eliminate redundancy and improve readability.

---

### 🤞 Testing Requirements
- Unit and collective tests validated with expected results.
- Visual acceptance tests (`SilkRoadATest`) allowing direct user verification in BlueJ.
- All constructors and key methods manually and visually verified.

---

## 5. Running the Project (BlueJ)

1. Open the project in **BlueJ**.
2. Ensure the `shapes` package is available.
3. Compile the classes in the following order:

## Authors

- **Camilo Aguirre**  
- **Mateo Sánchez**

Students of Systems Engineering  
Escuela Colombiana de Ingeniería Julio Garavito

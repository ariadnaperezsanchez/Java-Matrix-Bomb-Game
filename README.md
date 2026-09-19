# 💣 Java Matrix Bomb Game

Java Matrix Bomb Game is a console-based application developed in **Java** that combines matrix manipulation, random numbers, user input, and basic game logic.

The player creates a matrix with a custom number of rows and columns. Each cell is filled with a random value, and the player can place bombs at different coordinates to calculate explosion values and modify the matrix.

This project was developed as part of my Web Application Development studies to practice Java fundamentals, multidimensional arrays, loops, collections, and input validation.

---

## 🎮 How It Works

When the program starts, the user chooses the number of rows and columns for the matrix.

Both values must be greater than zero.

The application then creates a matrix and fills each cell with a random number between **0 and 9**.

Example:

```text
4 7 2 9
1 5 8 3
6 2 4 7
9 1 3 5
```

The user can then interact with the matrix through a console menu.

---

## ✨ Features

- Custom matrix dimensions
- Random matrix generation
- Input validation for rows and columns
- Display the current matrix
- Place bombs using coordinates
- Validate bomb coordinates
- Calculate explosion values
- Modify rows and columns after an explosion
- Reset the complete matrix
- Store explosion values
- Display explosion history
- Interactive console menu

---

## 📋 Menu

The application provides the following options:

```text
[1] Show matrix
[2] Place bomb
[3] Set all matrix values to 0
[4] Ranking
[0] Exit
```

---

## 💥 Bomb System

The player selects a position using X and Y coordinates.

For example:

```text
X: 2
Y: 3
```

If the coordinates are valid, the program calculates the explosion value using the selected position and its surrounding cells.

Conceptually:

```text
┌───┬───┬───┐
│ X │ X │ X │
├───┼───┼───┤
│ X │ 💣│ X │
├───┼───┼───┤
│ X │ X │ X │
└───┴───┴───┘
```

Cells outside the matrix boundaries are automatically ignored.

After calculating the explosion, the program sets the selected row and column to `0`.

---

## 🏆 Explosion Ranking

Each calculated explosion value is stored in an `ArrayList`.

The user can display the recorded explosion values using the ranking option:

```text
Explosion 1: 35
Explosion 2: 22
Explosion 3: 41
```

The ranking exists during the current execution of the application.

---

## 🔄 Reset Matrix

The user can reset the entire matrix.

When this option is selected, every value becomes:

```text
0
```

This demonstrates how nested loops can be used to modify every element of a two-dimensional array.

---

## 🛠️ Technologies

- Java
- Java Collections
- Multidimensional Arrays
- `ArrayList`
- `Random`
- `Scanner`
- Git
- GitHub

---

## 📁 Project Structure

```text
Java-Matrix-Bomb-Game/
└── src/
    └── SanchezPerezAriadna1.java
```

The main Java class contains:

- User input validation
- Matrix creation
- Random value generation
- Menu logic
- Bomb calculations
- Matrix modification
- Explosion history

---

## ▶️ Running the Project

### Requirements

Make sure Java is installed:

```bash
java -version
```

Check that the Java compiler is available:

```bash
javac -version
```

### Compile

From the project directory:

```bash
javac -d out src/*.java
```

### Run

Run the application with:

```bash
java -cp out SanchezPerezAriadna1
```

---

## 🧠 Concepts Practiced

This project demonstrates experience with:

- Java fundamentals
- Two-dimensional arrays
- Nested loops
- `while` loops
- `switch` statements
- Conditional statements
- User input with `Scanner`
- Input validation
- Random number generation
- Java collections
- `ArrayList`
- Matrix manipulation
- Coordinate validation
- Basic game logic

---

## 🎯 Project Purpose

Java Matrix Bomb Game was developed as an academic Java exercise during my Web Application Development studies.

The main objective was to practice working with two-dimensional arrays and nested loops while creating an interactive console application.

It also provided practice with collections, random values, user input, coordinate systems, and matrix manipulation.

---

## 🔮 Possible Future Improvements

Possible improvements include:

- Sort explosion values to create a real ranking
- Improve menu input validation
- Represent bombs separately from zero values
- Add player names
- Add a scoring system
- Add difficulty levels
- Add different bomb types
- Save rankings between executions
- Refactor the program into multiple classes
- Add automated tests
- Create a graphical user interface

---

## 👩‍💻 Author

**Ariadna Pérez Sánchez**

GitHub: `ariadnaperezsanchez`

# Soccer Match Simulator

## Project Description

The Soccer Match Simulator is a Python program that simulates a 90-minute soccer match between two teams. The program randomly generates shooting opportunities, determines whether shots are on target, tracks goals, and displays the final score and team statistics.

This project demonstrates object-oriented programming concepts, including classes, constructors, methods, variables, loops, and conditional statements.

## Features

- Simulates a 90-minute soccer match
- Generates random shooting opportunities
- Tracks goals, total shots, and shots on target
- Displays match events and the halftime score
- Shows the final score and team statistics
- Announces the winner or a draw

## Technologies Used

- Python 3
- Python random module

## How to Run the Program

1. Install Python 3 if it is not already installed.
2. Open the project folder in Visual Studio Code.
3. Open a terminal in the project folder.
4. Run the following command:

```bash
python soccer_simulator.py
```

On Windows, you can also try `py soccer_simulator.py`.

## Classes and Methods

### Team

The Team class represents a soccer team.

- `__init__()` initializes the team's name and statistics.
- `take_shot()` simulates a shot and updates the team's statistics.
- `display_stats()` displays the team's statistics.

### SoccerMatch

The SoccerMatch class manages the match between two teams.

- `__init__()` initializes both teams and the match duration.
- `simulate_match()` runs the match simulation.
- `display_score()` displays the current score.
- `display_winner()` determines the winner or draw.

## Assumptions

- The match lasts 90 minutes.
- The simulation advances in five-minute intervals.
- Each team has a 60% chance of getting a shooting opportunity at each interval.
- A shot has a 40% chance of being on target.
- A shot on target has a 30% chance of becoming a goal.

## Limitations

This is a simplified soccer simulation. It does not model individual players, tactics, possession, substitutions, extra time, or penalty shootouts. Results are randomly generated.

## Project Files

- `soccer_simulator.py` - Python source code
- `flowchart.md` - Program flowchart
- `pseudocode.md` - Program pseudocode
- `README.md` - Project documentation

## Author

Python OOP Midterm Project
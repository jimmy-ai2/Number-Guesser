# Number Guessing Game

A command-line guessing game where the player sets their own difficulty by defining the number range, then tries to guess a randomly generated number with directional hints along the way.

---

## Features

- **Player-Defined Range:** The player chooses the upper limit of the number range before the game begins, giving them control over the difficulty.
- **Random Number Generation:** A random number is generated within the chosen range at the start of each session, ensuring a unique game every time.
- **Directional Hints:** After each wrong guess, the game tells the player whether they guessed too high or too low, helping them zero in on the answer.
- **Guess Counter:** Tracks the total number of guesses taken and displays the final count once the correct number is found.
- **Input Validation:** Handles non-numeric and out-of-range inputs gracefully — invalid range values exit cleanly, and invalid guesses prompt a retry without crashing.

---

## Tech Stack

- **Python 3:** Core language powering all game logic, input handling, and output formatting.
  - **`random` module:** Used to generate an unpredictable number within the player's chosen range via `random.randint()`.
  - **`while` Loop:** Keeps the guessing loop running until the correct answer is found.
  - **`.isdigit()`:** Validates both the range input and each guess to ensure only numeric values are processed.
  - **f-Strings:** Used to deliver the final guess count in a clean, readable format.

---

## How to Use

1. **Run the Script:** Execute the file from your terminal with `python number-guesser.py`.
2. **Set Your Range:** Enter any positive number to define the upper limit of the guessing range.
3. **Make Guesses:** Type a number and press Enter — the game will tell you if you're too high or too low.
4. **Keep Guessing:** Use the hints to narrow down your answer until you land on the correct number.
5. **See Your Result:** Once correct, the game displays how many guesses it took you to win.

---

## Future Improvements

- **Limited Attempts Mode:** Cap the number of guesses based on the chosen range to add stakes and strategy.
- **Difficulty Presets:** Offer Easy, Medium, and Hard modes with predefined ranges so players can jump straight in.
- **Replay Option:** Prompt the player to start a new round after finishing instead of exiting the program.
- **Best Score Tracking:** Save the fewest guesses achieved for a given range so players can challenge their own records.

---

## 👤 About

This project was developed as a foundational Python exercise to demonstrate core programming concepts including randomness, input validation, and loop control. It prioritizes **simple, clean logic** — showing how a fun, interactive experience can be built with just a few core language features.

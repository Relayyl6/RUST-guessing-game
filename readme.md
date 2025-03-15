# Rust Guessing Game

A simple command-line number guessing game written in Rust. The program generates a random number between 1 and 100, and the player must guess the correct number. The game provides feedback on whether the guess is too high, too low, or correct.

## Features

- Generates a random number between 1 and 100.
- Provides feedback on each guess (too high, too low, or correct).
- Handles invalid input gracefully (non-numeric input is ignored).
- Loops until the correct number is guessed.

## How to Use

1. **Clone the repository** (if applicable) or copy the code into your Rust project.
2. **Run the program** using the following command:
   ```bash
   cargo run
   ```
3. **Follow the prompts**:
   - Enter your guess (a number between 1 and 100).
   - The program will tell you if your guess is too high, too low, or correct.
4. **Keep guessing** until you find the correct number.

## Example

```bash
$ cargo run
   Compiling guessing_game v0.1.0
    Finished dev [unoptimized + debuginfo] target(s) in 0.50s
     Running `target/debug/guessing_game`
Guess the number!
Please input your guess.
50
You guessed: 50
The secret number is 42
Too big
Please input your guess.
30
You guessed: 30
The secret number is 42
Too small
Please input your guess.
42
You guessed: 42
The secret number is 42
You win!
```

## Code Overview

The program uses Rust's standard library (`std::io`) to handle user input and the `rand` crate to generate a random number. It compares the user's guess to the secret number and provides feedback until the correct number is guessed.

### Key Functions

- **`rand::thread_rng().gen_range(1..=100)`**: Generates a random number between 1 and 100.
- **`io::stdin().read_line()`**: Reads input from the command line.
- **`trim()`**: Removes whitespace from the input.
- **`parse()`**: Converts the input string into an unsigned 32-bit integer.
- **`match guess.cmp(&secret_number)`**: Compares the guess to the secret number and provides feedback.

## Requirements

- Rust installed on your system. If not, follow the instructions at [rustup.rs](https://rustup.rs/).
- The `rand` crate added to your `Cargo.toml` file:
  ```toml
  [dependencies]
  rand = "0.8"
  ```

## Running Tests

This project does not currently include automated tests. However, you can manually test the program by running it and providing different inputs.

## Contributing

Contributions are welcome! If you'd like to improve this project, feel free to open an issue or submit a pull request.

## License

This project is open-source and available under the [MIT License](LICENSE.md).


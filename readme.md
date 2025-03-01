# Guessing Game  

A simple number guessing game implementation in Rust, created as a learning exercise from Chapter 2 of *The Rust Programming Language* book.  

**Features**:  
- Generates a random secret number between 1-100  
- Prompts user for input guesses  
- Provides feedback on whether guess is too high or too low  
- Validates user input  
- Tracks number of attempts  

This project demonstrates basic Rust concepts including:  
- Variables and data types  
- User input/output with `std::io`  
- Error handling with `Result`  
- Basic control flow with `match` and loops  
- Using external crates (`rand`)  

## How to Play  
1. The game generates a random number (1-100)  
2. Enter your numeric guess when prompted  
3. Receive feedback if your guess is too high/low  
4. Continue guessing until you find the correct number  

## Build & Run  
```bash 
cargo build
cargo run
```  

*Requires Rust toolchain and Cargo installed*  

## Example  
```text
Guess the number!
Please input your guess: 50
Too small!
Please input your guess: 75
Too big!
Please input your guess: 63
You won!
```  

This project was created following the official Rust Book tutorial to learn fundamental Rust programming concepts.  



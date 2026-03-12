# Hangman

## Demo

```
--------------------------
 Welcome to Java Hangman!
--------------------------

Word: _ _ _ _ _ _
Guess a letter: a

Correct!

Word: _ a _ a _ a
Guess a letter: z

Incorrect!

       O

Word: _ a _ a _ a
Guess a letter: n

Correct!

Word: _ a n a n a
Guess a letter: b

Correct!

YOU WIN!
The word was banana
```

## How to Run

### Prerequisites
- Java JDK 17+
- A file called `words` in the project root (one word per line)

### Example `words` file
```
banana
guitar
planet
rocket
puzzle
```

### Run the program
```bash
git clone https://github.com/elio-commits/Hangman-Game.git
cd Hangman-Game
javac Main.java
java Main
```

## Concepts Practiced

- Reading from a file using `BufferedReader` and `FileReader`
- Exception handling with `try-catch` (`FileNotFoundException`, `IOException`)
- `ArrayList` for storing the word list and tracking revealed letters
- String manipulation with `indexOf()` and `charAt()`
- Enhanced `switch` expressions with text blocks for ASCII art
- Game loop logic using a `while` loop and win/loss conditions

## Known Issues

- Guessing the same letter twice counts as a correct guess but doesn't warn the player
- Entering more than one character only reads the first letter with no feedback
- No replay option — the program exits after one round

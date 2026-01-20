# Pokemon Guessing Game

A fun interactive command-line Pokemon guessing game built with Python. Test your Pokemon knowledge by guessing the name of a Pokemon based on its ASCII art!

## Features

- 🎮 **Three Difficulty Levels**: Easy, Medium, and Hard
- 🎨 **ASCII Art Display**: Beautiful ASCII art representations of Pokemon
- 📊 **Score Tracking**: Your scores are saved locally and persist between sessions
- 🌈 **Colorful Terminal Output**: Enhanced visual experience with colored text
- 💾 **Progress Saving**: Scores are stored in your AppData directory

## Game Rules

1. You'll be shown the ASCII art of a Pokemon
2. You have **3 attempts** to guess the correct Pokemon name
3. Enter your guess in lowercase
4. Points are awarded based on difficulty:
   - **Easy**: 1 point per correct guess
   - **Medium**: 2 points per correct guess
   - **Hard**: 3 points per correct guess
5. Your total scores are saved automatically

## Installation

### Download Executable
Click the button to download the latest release.
[![Download](https://img.shields.io/badge/Download-EXE-brightgreen)](https://github.com/Arth-Joshi1001/POKEMON-GUESS-GAME/releases/download/GUESS-THE-POKEMON-1.0/pokemon.exe)

## Usage

The game will:
1. Display the ASCII art of a Pokemon
2. Prompt you to select a difficulty level (easy/medium/hard)
3. Ask for your guess
4. Display whether you're correct or give you remaining attempts
5. Track your score across sessions

## Project Structure

```
pokemon game/
├── pokemon.py          # Main game script
├── pokemon.spec        # PyInstaller specification file
├── score.txt          # Score file (auto-generated)
├── README.md          # This file
└── data/              # Pokemon data files
    ├── pikachu.txt
    ├── charizard.txt
    ├── blastoise.txt
    ├── gengar.txt
    ├── bulbasaur.txt
    ├── charmander.txt
    ├── chikorita.txt
    ├── eve.txt
    ├── jigllypuff.txt
    ├── mewtwo.txt
    ├── psyduck.txt
    ├── squritle.txt
    ├── snorlax.txt
    ├── easy.txt        # Easy mode Pokemon list
    ├── medium.txt      # Medium mode Pokemon list
    └── hard.txt        # Hard mode Pokemon list
```

## Score Storage

Scores are automatically saved in your system's AppData directory:
- **Windows**: `%APPDATA%\PokemonGuessGame\score.txt`

The file is created automatically on first run with initial scores of 0 for each difficulty level.

## Color Scheme

The game uses colored text for better visual feedback:
- 🟡 **Yellow**: General game information
- 🟢 **Green**: Success messages and ASCII art
- 🔴 **Red**: Error messages and game over
- 🔵 **Cyan**: User prompts and questions
- ⚪ **White**: Additional text

## Functions Overview

- `play()` - Main game loop for one round
- `main()` - Overall game controller
- `load(level)` - Loads Pokemon list for selected difficulty
- `load_asci(name)` - Loads ASCII art for a Pokemon
- `load_scores()` - Retrieves saved scores
- `save_scores(scores)` - Saves current scores
- `resource_path(relative_path)` - Handles PyInstaller compatibility
- Color functions (`yellow()`, `green()`, `red()`, `blue()`, `white()`) - Terminal color output

## Tips for Playing

- Pay close attention to the ASCII art details
- Think about distinctive features of each Pokemon
- Try easy mode first to get familiar with the game
- Challenge yourself with hard mode for higher scores

## Troubleshooting

**Q: The game won't start**
- Ensure Python 3.6+ is installed
- Check that all files are in the correct directory
- Try running from command prompt with full path

**Q: Scores aren't saving**
- Check if AppData directory exists and is writable
- Ensure you have proper permissions for AppData folder

**Q: ASCII art isn't displaying correctly**
- Make sure your terminal supports UTF-8 encoding
- Try a modern terminal emulator (Windows Terminal, etc.)

## 📬 Contact & Socials 

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/arth-joshi-8a37652aa)
[![Email](https://img.shields.io/badge/Email-Contact-red?style=for-the-badge&logo=gmail)](mailto:joshiarth646@gmail.com)

## License

This project is created for educational and entertainment purposes.

## Contributing

Feel free to fork, enhance, and submit improvements!

---

**Enjoy guessing! 🎮✨**

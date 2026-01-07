# Java Minesweeper

A simple, classic implementation of Minesweeper written in Java. This repository contains the game logic and a (console / GUI) implementation so you can play, learn from the code, and extend it.

> If this project has a different structure (for example a specific package name, build tool, or GUI framework), update the run/build instructions below accordingly. If you'd like, I can inspect the repo and tailor the README to the exact project files.

## Features

- Standard Minesweeper gameplay (reveal cells, flag mines)
- Multiple difficulty levels (beginner / intermediate / expert) or customizable board size and mine count
- Safe first-click behavior (first reveal won't be a mine)
- Recursive reveal of empty cells
- Win / lose detection and basic score/time tracking

## Requirements

- Java 8 or later
- (Optional) Maven or Gradle if the project uses a build tool

## Installing / Building

Option A — If the project provides a build tool (Maven or Gradle)

1. Clone the repository:

   ```bash
   git clone https://github.com/Abhi-39/Java_Minesweeper.git
   cd Java_Minesweeper
   ```

2. Build with Maven:

   ```bash
   mvn clean package
   ```

   or with Gradle:

   ```bash
   ./gradlew build
   ```

3. Run the generated JAR (if the project produces one):

   ```bash
   java -jar target/Java_Minesweeper.jar
   # or
   java -jar build/libs/Java_Minesweeper.jar
   ```

Option B — Plain Java (no build tool)

1. Compile the sources (adjust the path to your .java files):

   ```bash
   javac -d out $(find src -name "*.java")
   ```

2. Run the main class (replace com.example.Main with the actual main class):

   ```bash
   java -cp out com.example.Main
   ```

If you tell me the project's main class or build tool I can update these commands to match precisely.

## Running the Game

- Left-click (or primary action) to reveal a cell.
- Right-click (or secondary action) to place or remove a flag marking a suspected mine.
- Numbers indicate how many mines are adjacent to that cell.
- Revealing a mine ends the game (loss). Revealing all non-mine cells wins the game.

## Configuration

- Board size: Default sizes commonly provided are 9x9 (Beginner), 16x16 (Intermediate), and 30x16 (Expert).
- Mine count: Can be configured per difficulty or custom board.

## Testing

If the repository contains unit tests (JUnit or similar), run them with your build tool:

```bash
mvn test
# or
./gradlew test
```

## Contributing

Contributions, issues, and feature requests are welcome! Please follow these steps to contribute:

1. Fork the repository
2. Create a new branch for your change:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. Make your changes and add tests where appropriate
4. Commit your changes and push the branch

   ```bash
   git commit -am "Add feature: ..."
   git push origin feature/your-feature-name
   ```

5. Open a pull request with a clear description of your changes.

## License

This project is provided under the MIT License — see the LICENSE file for details. If no license is present, add one or change this section to the appropriate license.

## Author

- Abhi-39 — https://github.com/Abhi-39

---

If you'd like, I can:

- Inspect the repository and update this README with exact build/run commands and the main class name.
- Add usage screenshots or GIFs if a GUI exists (you can upload images to the repo).
- Add a CONTRIBUTING.md, CODE_OF_CONDUCT, or badges (build/test coverage).

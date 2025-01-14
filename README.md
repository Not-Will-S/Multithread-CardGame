# Multi-Threaded Card Game Project

This project is a multi-threaded card game application developed collaboratively using pair programming. The game involves players drawing and passing cards, with the objective of meeting a specific win condition. It leverages Java's multithreading capabilities, synchronized blocks, and file I/O operations to simulate concurrent gameplay.

## Features

### Core Functionality

- **Card Management**: Implementation of `Card`, `Deck`, and `Hand` classes to manage game components.
- **Player Interaction**: Players draw cards from decks and pass them to adjacent decks according to the game's rules.
- **Win Condition**: A player wins when all cards in their hand are of the same value.

### Multithreading

- **Thread Management**: Each player runs as a separate thread to simulate concurrent actions.
- **Thread Synchronization**: Synchronized blocks ensure thread safety when accessing shared resources, such as decks and hands.
- **Volatile Variables**: Used to handle shared variables across threads, ensuring proper visibility of changes.

### File Handling

- **Logging Actions**: Each player logs their actions to a separate file, providing a detailed game history.
- **Pack Shuffling**: Card packs are shuffled by reading and writing files.

### Exception Handling

- Robust handling of input errors, such as invalid player numbers and incorrect card pack formats.

### Design Patterns

- **Observer Pattern**: The `gameUpdates` class acts as a logging observer, recording game events.

## Skills Demonstrated

### 1. Java Programming

- Object-oriented design with encapsulated classes (`Card`, `Deck`, `Hand`, `Player`, `CardGame`, `GameUpdates`).
- Use of constructors, methods, and overridden methods such as `toString()`.

### 2. Multithreading & Concurrency

- Created and managed multiple threads using the `Runnable` interface.
- Implemented thread-safe operations with synchronized blocks and locks.
- Ensured data consistency with volatile and atomic variables (`AtomicInteger`).

### 3. File I/O

- Read from and wrote to files using `BufferedReader`, `BufferedWriter`, and `FileWriter`.
- Managed file operations efficiently by handling exceptions and closing resources properly.

### 4. Problem Solving

- Designed and implemented game rules with careful consideration of edge cases, such as:
  - Ensuring valid card distribution.
  - Handling empty decks and hands.

### 5. Collaboration & Agile Development

- Developed using pair programming techniques to enhance code quality and shared understanding.
- Followed an iterative development approach with frequent testing and code reviews.

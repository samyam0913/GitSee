# Git Visualization

**An interactive C++ desktop application for understanding Git concepts through real-time graphical visualization.**

Git Visualization is an educational tool designed to make learning Git easier, particularly for beginners. It allows users to enter Git commands through a graphical interface and observe how operations affect commit history, branches, and repository structures.

Rather than relying entirely on command-line explanations, the application uses visual representations and fundamental data structures to demonstrate how Git workflows operate.

## Application Preview

<!-- Replace these paths with your actual screenshots -->

<p align="center">
  <img src="screenshots/gitsee_demo.webp" alt="GitSee - Git Visualization Main Interface" width="850">
</p>

<p align="center">
  <em>Main application interface</em>
</p>

## Key Features

- **Interactive GUI:** Execute Git commands directly through the graphical interface.
- **Real-Time Visualization:** Observe changes in commit history and branching structures as commands are executed.
- **Git Command Interpretation:** Parse and process commands such as `git init`, `git commit`, `git branch`, `git checkout`, and `git merge`.
- **Commit History Visualization:** Represent commit relationships using linked lists and graphs.
- **Branch Management:** Visualize branches and their associated commits.
- **File-System Representation:** Model repository file and directory hierarchies using tree structures.
- **Error Handling:** Display feedback for invalid commands and incorrect inputs.

## Data Structures Used

The application integrates fundamental data structures to represent different aspects of Git:

| Data Structure | Application |
|---|---|
| Doubly Linked Lists | Represent commit history and commit relationships |
| Maps | Maintain branch names and their associated commit references |
| Graphs | Represent commit relationships, branching, and merging |
| Trees | Represent file and directory hierarchies within commits |

These structures help demonstrate how different Git operations affect repository state.

## Technical Architecture

The application follows a modular C++ architecture:

- **GUI Module (`guiLogic`):** Handles graphical rendering and user interaction.
- **Input Module (`Input`):** Manages user input and command handling.
- **Parser Module (`Parser`):** Processes command strings and extracts commands and arguments.
- **DSA Module (`DSA`):** Implements the data structures used to represent Git concepts.
- **Main Module (`main`):** Provides the application entry point and coordinates the application components.

## Technology Stack

- **Programming Language:** C++
- **Graphics Library:** SFML 2.5.1
- **IDE:** Microsoft Visual Studio
- **Data Structures:** Doubly Linked Lists, Maps, Graphs, Trees
- **Build Environment:** Visual Studio / MSBuild

## Project Structure

```text
Git-Visualizer/
│
├── Dependencies/
│   └── SFML-2.5.1/
│       ├── include/
│       └── lib/
│
├── headers/
│   ├── DSA.hpp
│   ├── guiLogic.hpp
│   ├── Input.hpp
│   └── Parser.hpp
│
├── src/
│   ├── DSA.cpp
│   ├── guiLogic.cpp
│   ├── Input.cpp
│   ├── main.cpp
│   └── Parser.cpp
│
├── screenshots/
├── arial.ttf
├── bg.jpg
├── logo.png
│
├── Git_visualisation.sln
├── Git_visualisation.vcxproj
└── Git_visualisation.vcxproj.filters
```

## Getting Started

### Prerequisites

- Windows 10 or later
- Microsoft Visual Studio 2019 or later
- Desktop development with C++ workload
- SFML 2.5.1

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/samyam0913/GitSee.git
   ```

2. Navigate to the project directory:

   ```bash
   cd GitSee
   ```

3. Open `Git_visualisation.sln` using Visual Studio.

4. Ensure that SFML 2.5.1 is configured correctly in the project settings and that its dependency paths are valid.

5. Select the appropriate build configuration (Debug or Release) and platform (x64).

6. Build and run the application.

> **Note:** The project currently includes SFML dependencies configured for Windows. Additional configuration may be necessary when using a different development environment.

## Limitations

- The application focuses on selected fundamental Git commands rather than the complete Git command set.
- Advanced Git workflows and edge cases may not be fully represented.
- The current implementation is designed around a graphical learning environment rather than a complete replacement for Git's native CLI.

## Future Improvements

- Support additional Git commands and advanced workflows.
- Introduce interactive, step-by-step Git tutorials.
- Improve visualization customization and user interaction.
- Explore integration with online Git repositories.
- Extend compatibility to Linux and other operating systems.

## Acknowledgements

This project was developed as an academic project with guidance from **Mr. Prakash Chandra Prasad**, Assistant Professor at IOE, Pulchowk Campus. 

We also acknowledge the contributions and feedback of our classmates and collaborators throughout the development process.

### Developed by
**Samyam Giri, Biplob Giri, Amit Aacharya, Sandip Acharya**

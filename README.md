# Folder Flow

A lightweight Java utility that creates a project folder, adds custom subfolders, and opens the finished project directly in Visual Studio Code.

Folder Flow includes both a command-line workflow and a Swing desktop interface. It was built to remove repetitive setup work from small web and software projects.

## Features

- Creates a named project directory.
- Creates any number of custom subfolders.
- Opens the finished directory in Visual Studio Code.
- Provides CLI and desktop GUI versions.
- Validates project names in the GUI.
- Uses a separate `ProjectBuilder` service class for file-system operations.

## Built with

- Java
- Java Swing
- `Scanner`
- `File`
- `ProcessBuilder`

## Run the command-line version

```bash
javac FolderCreator.java
java FolderCreator
```

## Run the desktop version

Compile the GUI and its service class:

```bash
javac FolderCreatorGUI.java ProjectBuilder.java
java FolderCreatorGUI
```

Visual Studio Code must be installed and its `code` command must be available in your Windows PATH.

## Example

Input:

```text
Project name: client-website
Folders: assets, css, js, images
```

Output:

```text
client-website/
├── assets/
├── css/
├── images/
└── js/
```

## Skills demonstrated

- Object-oriented Java
- User-input handling and validation
- Loops and collections of values
- File-system automation
- Process execution
- Event-driven Swing interfaces
- Separation between UI and service logic

## Current limitation

The VS Code launcher currently targets Windows. Cross-platform launch support and automated project templates are planned improvements.

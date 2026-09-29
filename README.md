# Text Editor App in Python

A simple desktop **Text Editor application built with Python and Tkinter**.
This project demonstrates basic GUI development, file handling, menus, functions, and event-driven programming in Python.

## Features

* Create a new text document
* Open existing `.txt` files
* Edit text inside the application
* Save text as a `.txt` file
* File menu with New, Open, Save, and Exit options
* Popup message after successfully saving a file
* Resizable text editing area
* Word wrapping for better readability

## Technologies Used

* **Python 3**
* **Tkinter**
* File Handling
* GUI Programming
* Event-Driven Programming

## Python Concepts Demonstrated

### 1. Tkinter

Tkinter is Python's built-in library for creating graphical user interfaces.

```python
import tkinter as tk
```

It provides components such as windows, text boxes, menus, buttons, and dialogs.

### 2. File Dialogs

The `filedialog` module is used to allow users to select files from their computer.

```python
filedialog.askopenfilename()
filedialog.asksaveasfilename()
```

### 3. Message Boxes

The `messagebox` module displays popup messages to the user.

```python
messagebox.showinfo("Info", "File saved successfully!")
```

### 4. Text Widget

The `Text` widget provides a multi-line area where users can write and edit text.

```python
text = tk.Text(root, wrap=tk.WORD)
```

### 5. File Handling

The project uses Python's `open()` function to read and write files.

```python
with open(file_path, "r") as file:
    data = file.read()
```

For saving:

```python
with open(file_path, "w") as file:
    file.write(data)
```

### 6. Functions

Separate functions are created for different operations:

* `new_file()` → clears the editor
* `open_file()` → opens an existing text file
* `save_file()` → saves the current text

### 7. Menu Bar

A menu bar is created using Tkinter's `Menu` widget.

The **File** menu contains:

* New
* Open
* Save
* Exit

### 8. Event-Driven Programming

The application responds to user actions such as selecting menu options, opening files, saving files, and closing the application.

## How to Run

### Prerequisites

Make sure Python 3 is installed on your system.

Check your Python version:

```bash
python --version
```

Tkinter is included with most standard Python installations.

### Run the Application

Clone the repository:

```bash
git clone https://github.com/your-username/text-editor-python.git
```

Go to the project directory:

```bash
cd text-editor-python
```

Run the application:

```bash
python text_editor.py
```

## Project Structure

```text
text-editor-python/
│
├── text_editor.py
└── README.md
```

## How It Works

1. The application creates a main Tkinter window.
2. A text area is added for writing and editing content.
3. The File menu provides New, Open, Save, and Exit options.
4. When **Open** is selected, the user chooses a `.txt` file and its contents are loaded into the editor.
5. When **Save** is selected, the user chooses a location and the current text is written to a `.txt` file.
6. The application continues running through Tkinter's event loop until the user closes it.

## Future Improvements

Some features that can be added in the future:

* Cut, Copy, and Paste
* Undo and Redo
* Keyboard shortcuts
* Find and Replace
* Font and text-size customization
* Dark mode
* Support for additional file formats

## Learning Outcome

Through this project, I learned how to:

* Build a basic desktop GUI using Tkinter
* Work with files using Python
* Create and use functions
* Create menus and submenus
* Use file dialogs and message boxes
* Understand event-driven programming
* Structure a small Python application

## License

This project is created for learning and educational purposes.

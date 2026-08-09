# HK-Calculator

A modular **scientific calculator built with Python and Tkinter**, featuring advanced mathematical functions, calculation history, themes, memory operations, and keyboard controls.

## Features

- Basic arithmetic operations
- Scientific functions including `sin`, `cos`, `tan`, `log`, `ln`, and square root
- Powers, factorials, constants, and additional mathematical operations
- Primary and secondary function modes
- Degree and radian modes
- Memory operations (`M+`, `M-`, `MR`, `MC`)
- Calculation history
- Light and dark themes
- Keyboard shortcuts
- Responsive interface
- Standalone Windows executable support

## Project Structure

```text
HK-Calculator/
├── docs/
│   ├── HK.ico
│   ├── HK_png.png
│   └── screenshots/
│
├── src/
│   ├── main.py
│   ├── logic.py
│   ├── utils.py
│   └── yi_config.py
│
├── .gitignore
└── README.md
```

The application is separated into modules for the user interface, calculator logic, utility functions, and configuration to keep the code organized and maintainable.

## Run from Source

### Requirements

- Python 3
- Tkinter

Clone the repository:

```bash
git clone https://github.com/alihk1684/HK-Calculator.git
cd HK-Calculator
```

Run the application:

```bash
python src/main.py
```

## 🖼️ Screenshots

![Dark Mode Default](docs/dark_mode_default_view.png)
![Dark Mode + History](docs/dark_mode_history_panel.png)
![Light Mode + History](docs/light_mode_history_panel.png)

## Keyboard Controls

| Key | Action |
|---|---|
| `0-9` | Enter digits |
| `+ - * /` | Basic operations |
| `Enter` / `=` | Calculate |
| `Backspace` | Delete character |
| `Esc` | Clear |
| `r` | Toggle radians/degrees |
| `q` | Toggle theme |
| `h` | Toggle history |

Additional shortcuts are available for scientific functions.

## Technical Highlights

- Modular Python architecture
- Tkinter GUI development
- Mathematical expression processing
- Input and syntax validation
- Event-driven programming
- Keyboard event handling
- Dynamic UI and font resizing
- Application state management
- PyInstaller executable packaging

## Build Windows Executable

The application can be packaged using PyInstaller:

```bash
pyinstaller --noconfirm --onefile --windowed ^
  --name=HK_Calculator ^
  --icon=docs/HK.ico ^
  --add-data "docs/HK_png.png;docs" ^
  src/main.py
```

The generated executable will be available in the `dist/` directory.

## Future Improvements

- Persistent calculation history
- Additional scientific functions
- Improved expression parsing
- More customization options
- Automated testing

## Author

**Ali Heidari**  
Electrical Engineering student.

## License

This project is available under the MIT License.

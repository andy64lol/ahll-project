# AHLL - Andy's Happy Little Language VSCode Extension

![AHLL Logo](https://img.shields.io/badge/AHLL-Andy's%20Happy%20Little%20Language-brightgreen) ![Version](https://img.shields.io/badge/version-0.0.1-blue) ![VSCode](https://img.shields.io/badge/VSCode-Extension-purple)

This VSCode extension provides language support for **AHLL (Andy's Happy Little Language)** - a whimsical programming language designed to make coding fun and happy!

## Features

- **Syntax Highlighting**: Full syntax highlighting for AHLL files (.ahll)
- **Code Recognition**: Automatic detection of .ahll files
- **Comment Support**: Single-line comments with `//`
- **Bracket Matching**: Auto-closing and matching for all brackets

## AHLL Language Features

AHLL is a fun, whimsical programming language with English-like syntax:

### Variables & Lists
```ahll
create_new_classroom_named_("my_vars")
add_new_student_with_name_of_("x")_to_classroom_("my_vars")
teach_("x")_a_bit_of_(42)_from_classroom("my_vars")
write_this([x])
```

### Input & Output
```ahll
write_this("Hello, World!")
ask_this("What is your name? ")
```

### Conditionals
```ahll
If_<("status")_is_("ready")>_then_do:
    write_this("Status is ready!")

but if_<the_following_thing_is_not_true_lol_<("status")_is_("done")>>_do:
    write_this("Status is NOT done")
```

### Loops
```ahll
do_this_(5)_times:
    write_this("Hello!")
```

### Time Delays
```ahll
STAY_THERE_AND_DONT_DARE_TO_MOVE_FOR_(2)_SECONDS
```

### Functions (Concepts)
```ahll
create_new_concept_("greet")
define_concept_("greet")_here:
    write_this("Hello from concept!")
```

### File I/O
```ahll
file_document_("data.txt")_as_("my_list")
burn_papers_("data.txt")
```

### Shell Integration
```ahll
use_cheating_("ls -la")
```

## Installation

### From VSCode Marketplace

1. Open VSCode
2. Press `Ctrl+Shift+X` (or `Cmd+Shift+X` on Mac) to open Extensions
3. Search for "AHLL" or "Andy's Happy Little Language"
4. Click Install

### From Source

1. Clone the repository:
   ```bash
   git clone https://github.com/andy64lol/ahll-project.git
   ```

2. Navigate to the VSCode extension folder:
   ```bash
   cd ahll-project/extension_vscode/andy-s-happy-little-language---ahll--support
   ```

3. Package the extension:
   ```bash
   npm install -g vsce
   vsce package
   ```

4. Install the `.vsix` file:
   ```bash
   code --install-extension ahll-*.vsix
   ```

### Manual Installation

Copy the extension folder to your VSCode extensions directory:
- **Windows**: `%USERPROFILE%\.vscode\extensions\`
- **macOS**: `~/.vscode/extensions/`
- **Linux**: `~/.vscode/extensions/`

## Usage

1. Create a new file with `.ahll` extension (e.g., `hello.ahll`)
2. Start coding in AHLL!
3. Run your program with:
   ```bash
   ahll hello.ahll
   # or
   bananacat hello.ahll
   ```

## Quick Example

```ahll
write_this("Welcome to AHLL!")

// Create a variable
create_new_classroom_named_("my_vars")
add_new_student_with_name_of_("greeting")_to_classroom_("my_vars")
teach_("greeting")_a_bit_of_("Hello, World!")_from_classroom("my_vars")

write_this([greeting])

// Loops
do_this_(3)_times:
    write_this("  Tick...")

// Time delays
STAY_THERE_AND_DONT_DARE_TO_MOVE_FOR_(1)_SECONDS
write_this("1 second later!")
```

## Requirements

- VSCode version 1.108.1 or higher
- Python 3 (to run AHLL programs)

## Extension Settings

This extension contributes the following settings:

* `ahll.enable`: Enable/disable AHLL language support (default: true)

## Known Issues

- No IntelliSense/autocomplete yet (coming in future versions)
- No hover tooltips yet (coming in future versions)

## Release Notes

### 0.0.1

Initial release of AHLL VSCode extension:
- Basic syntax highlighting for AHLL files
- Comment support
- Bracket matching
- File extension recognition

## For More Information

- **AHLL Repository**: https://github.com/andy64lol/ahll-project
- **AHLL Documentation**: See [docs.md](https://github.com/andy64lol/ahll-project/blob/main/docs.md) for complete language reference
- **VSCode Extension Documentation**: https://code.visualstudio.com/api/language-extensions/overview

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test the extension
5. Submit a pull request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*"Make coding fun again!"* - andy64lol 🌻🍌🐈


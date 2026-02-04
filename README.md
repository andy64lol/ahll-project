# AHLL - Andy's Happy Little Language

![AHLL Logo](https://img.shields.io/badge/AHLL-Andy's%20Happy%20Little%20Language-brightgreen) ![Version](https://img.shields.io/badge/version-1.0-blue) ![License](https://img.shields.io/badge/license-MIT-green)

Welcome to **AHLL** (Andy's Happy Little Language)! 🌻🍌🐈

AHLL is a whimsical, fun programming language designed to make coding feel like playing in a happy little classroom. Created by [andy64lol](https://github.com/andy64lol), it's perfect for beginners, educators, and anyone who wants to code with a smile.

## Features

- **Whimsical Syntax**: Commands like `write_this("Hello!")`, `create_new_classroom_named_("my_list")`, and `add_new_student_with_name_of_("x")_to_classroom_("my_list")` make coding playful and memorable.
- **Core Programming Concepts**: Variables, lists, math operations, input/output, conditionals, functions, and more.
- **File I/O**: Save and load data with `file_document_()` and `burn_papers_()`.
- **Shell Integration**: Run system commands with `use_cheating_()`.
- **Easy to Learn**: Simple, English-like syntax that's forgiving and fun.
- **Cross-Platform**: Runs on any system with Python 3.

## Installation

### Option 1: Debian Package (Recommended for Debian/Ubuntu)

1. Build the package:
   ```bash
   ./builder
   ```

2. Install the package:
   ```bash
   sudo dpkg -i ahll_1.0-1_all.deb
   ```

### Option 2: Manual Installation

1. Ensure Python 3 is installed on your system.

2. Copy the interpreter to your PATH:
   ```bash
   sudo cp usr/bin/ahll /usr/local/bin/
   sudo cp usr/bin/bananacat /usr/local/bin/
   sudo chmod +x /usr/local/bin/ahll /usr/local/bin/bananacat
   ```

3. (Optional) Install man pages:
   ```bash
   sudo cp usr/share/man/man1/ahll.1 /usr/local/share/man/man1/
   sudo cp usr/share/man/man1/bananacat.1 /usr/local/share/man/man1/
   sudo gzip /usr/local/share/man/man1/ahll.1 /usr/local/share/man/man1/bananacat.1
   sudo mandb
   ```

## Usage

### Running Programs

Use the `ahll` interpreter directly:
```bash
ahll example.ahll
```

Or use the fun `bananacat` wrapper:
```bash
bananacat example.ahll
```

### Command Line Options

- `ahll file.ahll`: Run an AHLL program
- `bananacat file.ahll`: Run an AHLL program with style
- `bananacat --help`: Show help
- `bananacat --version`: Show version

## Quick Example

Here's a simple AHLL program:

```ahll
write_this("Welcome to AHLL!")

// Create a variable
create_new_classroom_named_("my_vars")
add_new_student_with_name_of_("greeting")_to_classroom_("my_vars")
teach_("greeting")_a_bit_of_("Hello, World!")_from_classroom("my_vars")

write_this([greeting])

// Ask for input
ask_this("What's your name? ")
write_this("Nice to meet you, ")
write_this([answer])
```

Save this as `hello.ahll` and run it with `bananacat hello.ahll`.

For more examples, see the `example.ahll` file in this repository.

## Documentation

For detailed syntax reference, command guide, and advanced features, see [DOCS.md](DOCS.md).

## Contributing

AHLL is a labor of love! If you'd like to contribute:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly (AHLL programs should be happy!)
5. Submit a pull request

Ideas for contributions:
- New whimsical commands
- Performance improvements
- Bug fixes
- Documentation improvements
- Port to other platforms

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Credits

- **Creator**: [andy64lol](https://github.com/andy64lol)
- **Inspired by**: The joy of programming and happy little accidents

---

*"Make coding fun again!"* - andy64lol 🌻

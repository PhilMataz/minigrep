# Minigrep

A simple command-line search tool implemented in Rust, inspired by the classic `grep` utility. This project allows you to search for specific text patterns within files.

## Features

- Case-sensitive and case-insensitive search options
- File content searching with pattern matching
- Environment variable configuration support
- Error handling for file operations and invalid inputs

## Installation

Ensure you have Rust installed on your system. Then clone this repository and build the project:

```bash
git clone https://github.com/yourusername/minigrep
cd minigrep
cargo build --release
```

## Usage

Basic usage:

```bash
cargo run <search_pattern> <file_path>
```

Example:

```bash
cargo run to poem.txt
```

### Case Sensitivity

The search can be made case-insensitive by setting the `IGNORE_CASE` environment variable:

```bash
IGNORE_CASE=1 cargo run to poem.txt
```

## Environment Variables

- `IGNORE_CASE`: Set to `1` to enable case-insensitive search

## Error Handling

The program handles various error cases:

- Missing command line arguments
- File not found
- Permission errors
- Invalid UTF-8 content

## Project Structure

```
src/
├── main.rs       # Entry point and argument handling
└── lib.rs        # Core functionality and tests
```

## Contributing

Feel free to submit issues and pull requests to improve the functionality of this project.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Built as a learning project following the Rust Programming Language book
- Inspired by the GNU grep utility

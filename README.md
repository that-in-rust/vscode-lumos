# VS Code Lumos

A VS Code extension for syntax highlighting Java and Rust code blocks in .txt files.

## Features

- Syntax highlighting for Java code blocks in .txt files
- Syntax highlighting for Rust code blocks in .txt files
- Supports code blocks marked with triple backticks (```)

Example screenshot:

![alt text](<Screenshot from 2024-11-03 14-55-20.png>)

## Usage

In any .txt file:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
```

```rust
fn main() {
    println!("Hello World");
}
```

## Building the Extension

1. Clone the repository:
```bash
git clone https://github.com/that-in-rust/vscode-lumos.git
cd vscode-lumos
```

2. Install dependencies:
```bash
npm install
npm install -g @vscode/vsce
```

3. Generate VSIX file:
```bash
vsce package
```

This will create a `vscode-lumos-x.x.x.vsix` file in your project directory.

## Installation

Method 1 - Command Palette:
1. Press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac)
2. Type "Install from VSIX"
3. Select "Extensions: Install from VSIX..."
4. Choose the generated `.vsix` file

Method 2 - Extensions View:
1. Open VS Code
2. Go to Extensions view (Ctrl+Shift+X)
3. Select "Install from VSIX..." from the menu
4. Choose the generated `.vsix` file

## Requirements

- VS Code 1.80.0 or higher
- Node.js & npm for building

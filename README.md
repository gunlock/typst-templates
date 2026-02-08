# Typst Templates

A collection of Typst templates for various document types.

## What is Typst?

Typst is a modern markup-based typesetting system designed to be an alternative to LaTeX. It offers a cleaner syntax, faster compilation, and better error messages while maintaining powerful typesetting capabilities.

## Installing Typst

### Windows

**Option 1: Using winget (recommended)**

```bash
winget install --id Typst.Typst
```

**Option 2: Using Scoop**

```bash
scoop install typst
```

**Option 3: Manual installation**

1. Download the latest release from [Typst releases](https://github.com/typst/typst/releases)
2. Extract the archive and add the binary to your PATH

### macOS

**Option 1: Using Homebrew (recommended)**

```bash
brew install typst
```

**Option 2: Manual installation**

1. Download the latest release from [Typst releases](https://github.com/typst/typst/releases)
2. Extract the archive and move the binary to `/usr/local/bin`

### Linux

**Option 1: Using package manager**

For Arch Linux:

```bash
pacman -S typst
```

For Ubuntu/Debian (if available in repos):

```bash
apt install typst
```

**Option 2: Using Cargo (Rust package manager)**

```bash
cargo install --git https://github.com/typst/typst --locked typst-cli
```

**Option 3: Manual installation**

1. Download the latest release from [Typst releases](https://github.com/typst/typst/releases)
2. Extract the archive and move the binary to `/usr/local/bin` or `~/.local/bin`
3. Make it executable: `chmod +x typst`

## Fonts

The examples in this repository use the **Inter** font family, which provides excellent readability.

### Installing the Inter Font

**Download Inter:**

- GitHub Repository: https://github.com/rsms/inter
- Or download directly from [Google Fonts](https://fonts.google.com/specimen/Inter)

### Font Installation by Operating System

**Windows:**

1. Download and extract the font files
2. Select all `.ttf` or `.otf` files
3. Right-click and select "Install" or "Install for all users"
4. Alternatively, copy font files to `C:\Windows\Fonts`

**macOS:**

1. Download and extract the font files
2. Double-click each font file
3. Click "Install Font" in the Font Book preview
4. Alternatively, copy font files to `~/Library/Fonts` (user) or `/Library/Fonts` (system-wide)

**Linux:**

1. Download and extract the font files
2. Copy font files to `~/.local/share/fonts` (user) or `/usr/share/fonts` (system-wide)
3. Run `fc-cache -fv` to refresh the font cache

## Compiling Documents

To compile a Typst document to PDF:

```bash
typst compile input.typ output.pdf
```

To watch a file and automatically recompile on changes:

```bash
typst watch input.typ output.pdf
```

To compile with a specific output format:

```bash
typst compile input.typ output.png  # PNG image
typst compile input.typ output.svg  # SVG image
```

### Example Usage

```bash
# Compile a checklist
cd aviation
typst compile checklist-example.typ checklist-example.pdf

# Watch and auto-compile
typst watch checklist-example.typ checklist-example.pdf
```

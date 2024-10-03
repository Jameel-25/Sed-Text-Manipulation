# Sed-Text-Manipulation

A collection of examples and use cases for the `sed` (Stream Editor) command in Unix-based systems. This repository is designed to help users understand and apply various text manipulation techniques using `sed`.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
  - [Basic Find and Replace](#basic-find-and-replace)
  - [Delete Lines Matching a Pattern](#delete-lines-matching-a-pattern)
  - [Insert Text Before or After a Line](#insert-text-before-or-after-a-line)
  - [Advanced Pattern Matching](#advanced-pattern-matching)
- [Contributing](#contributing)
- [License](#license)

## Introduction

`sed` is a powerful command-line utility that allows you to filter and transform text in Unix-like operating systems. Whether you're processing configuration files, analyzing large datasets, or manipulating text, `sed` can perform complex text transformations with ease.

This repository contains a variety of examples and practical use cases to demonstrate the utility of `sed` in different scenarios.

## Features

- Basic and advanced text replacement
- Line deletion and insertion based on patterns
- Regular expression-based text processing
- In-place file editing
- Practical use cases for automation

## Installation

To use `sed`, make sure it is installed on your system. Most Unix-like operating systems come with `sed` pre-installed. You can verify this by running:

```bash
sed --version
```

If `sed` is not installed, you can install it using your package manager:

For Debian-based systems (Ubuntu, etc.):
```bash
sudo apt-get install sed
```

For Red Hat-based systems (CentOS, Fedora, etc.):
```bash
sudo yum install sed
```

For macOS using Homebrew:
```bash
brew install gnu-sed
```

## Usage

To run `sed` commands, use the following syntax:

```bash
sed [OPTIONS] 'command' file
```

Examples of common options:
- `-i`: Edit files in place
- `-e`: Specify multiple commands
- `-n`: Suppress automatic printing of the pattern space

## Examples

### Basic Find and Replace

Replace the first occurrence of a word:

```bash
sed 's/old-word/new-word/' input.txt
```

### Delete Lines Matching a Pattern

Remove lines that match a pattern:

```bash
sed '/pattern/d' input.txt
```

### Insert Text Before or After a Line

Insert a line of text before a match:

```bash
sed '/pattern/i\Insert this line' input.txt
```

### Advanced Pattern Matching

Replace text only if two conditions are met:

```bash
sed '/start/,/end/s/old/new/' input.txt
```

For more detailed examples, refer to the individual scripts in this repository.

## Contributing

If you'd like to contribute, feel free to submit a pull request. Whether it's fixing a bug, improving documentation, or adding new examples, your help is always appreciated!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

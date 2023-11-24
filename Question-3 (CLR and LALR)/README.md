# CLR(1) Parser Generator

This Python script implements a CLR(1) parser generator for a given context-free grammar. The parser generator uses the canonical LR(1) parsing technique to construct LR(1) parsing table.

## Requirements

Before using the script, make sure you have the following Python packages in yor directory:

```bash
from firstfollow.py import *
```

## Usage

```python
python clr1_parser_generator.py
```

## Description

The script defines classes and functions to generate a CLR(1) parsing table for a given context-free grammar. Here's an overview of the main components:

### State Class

- Represents a state in the LR(1) parsing automaton.
- Each state contains a closure, which is a set of LR(1) items.

### Item Class

- Represents an LR(1) item.
- Contains a production item and a lookahead set.

### Closure Function

```python
def closure(items):
    ...
```

- Computes the closure of a set of LR(1) items.

### Goto Function

```python
def goto(items, symbol):
    ...
```

- Computes the Goto operation for a set of LR(1) items and a given symbol.

### Calc_States Function

```python
def calc_states():
    ...
```

- Calculates all the states in the LR(1) parsing automaton.

### Make_Table Function

```python
def make_table(states):
    ...
```

- Constructs the CLR(1) parsing table.

### Augment_Grammar Function

```python
def augment_grammar():
    ...
```

- Augments the grammar to ensure it is suitable for CLR(1) parsing.

### Main Function

```python
def main():
    ...
```

- The main function that orchestrates the generation of the CLR(1) parsing table.
- Computes the FIRST and FOLLOW sets for non-terminals.
- Augments the grammar.
- Calculates states in the LR(1) automaton.
- Constructs and displays the CLR(1) parsing table.
- Detects shift/reduce and reduce/reduce conflicts.

## Acknowledgments

This script is inspired by the CLR(1) parsing technique and builds on the First-Follow computation provided by the `firstfollow` module.

## Contributing

- [Hamza Iftikhar - 21-CS-45](https://github.com/hamzaiftkhar)

If you'd like to contribute to this project, please follow the [Contributing Guidelines](CONTRIBUTING.md).
# LR(0) and SLR(1) Parsers for the Given Grammar

This repository contains the implementation of LR(0) and SLR(1) parsers for the provided grammar. Additionally, it includes the construction of the canonical collection of LR(0) items and the parsing table for both LR(0) and SLR(1) parsers.

## Grammar

```plaintext
E -> E + T | T
T -> T * F | F
F -> F / a | b
```

## Implementation Details

### 1. Canonical Collection of LR(0) Items

The LR(0) parser starts by computing the canonical collection of LR(0) items. This collection represents the LR(0) states in the parsing automaton.

**File:** `lr0_items.py`

```python
# Example Usage
# lr0_items.create_lr0_items(grammar)
```

### 2. LR(0) Parsing Table

The LR(0) parsing table is then generated based on the canonical collection of LR(0) items.

**File:** `lr0_parser_table.py`

```python
# Example Usage
# lr0_parser_table.create_lr0_parser_table(lr0_items)
```

### 3. SLR(1) Parsing Table

The SLR(1) parsing table is constructed using the canonical collection of LR(0) items and follow sets.

**File:** `slr1_parser_table.py`

```python
# Example Usage
# slr1_parser_table.create_slr1_parser_table(lr0_items, follow_sets)
```

## LR(0) or SLR(1)?

The given grammar is SLR(1) but not LR(0). The SLR(1) parser resolves conflicts that may arise in the LR(0) parser due to the usage of follow sets.

The SLR(1) parser is an enhanced version of the LR(0) parser, and it handles the shift-reduce and reduce-reduce conflicts more effectively by considering the follow sets of non-terminals.

Feel free to explore the code and run the scripts to observe the construction of LR(0) and SLR(1) parsers for the provided grammar.

## Contributors

- [Zunysha Naveed - 21-CS-75]()
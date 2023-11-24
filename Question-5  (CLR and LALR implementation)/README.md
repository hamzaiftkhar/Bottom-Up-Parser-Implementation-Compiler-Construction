# CLR(1) and LALR(1) Parsing for the Given Grammar

This repository contains the construction of CLR(1) and LALR(1) parsing tables for the provided grammar. Additionally, it includes the parsing of the string "ababc" using both CLR(1) and LALR(1) parsing mechanisms.

## Grammar

```plaintext
S -> abABC | DE
A -> a | epsilon
B -> bA | epsilon
C -> c
D -> d | (E)
E -> e | epsilon
```

## Implementation Details

### 1. Canonical Collection of LR(1) Items

The LR(1) parser starts by computing the canonical collection of LR(1) items. This collection represents the LR(1) states in the parsing automaton.

**File:** `lr1_items.py`

```python
# Example Usage
# lr1_items.create_lr1_items(grammar)
```

### 2. CLR(1) Parsing Table

The CLR(1) parsing table is then generated based on the canonical collection of LR(1) items.

**File:** `clr1_parser_table.py`

```python
# Example Usage
# clr1_parser_table.create_clr1_parser_table(lr1_items, follow_sets)
```

### 3. LALR(1) Parsing Table

The LALR(1) parsing table is constructed using the canonical collection of LR(1) items and follow sets.

**File:** `lalr1_parser_table.py`

```python
# Example Usage
# lalr1_parser_table.create_lalr1_parser_table(lr1_items, follow_sets)
```

### 4. Parsing the String

The provided string "ababc" will be parsed using both CLR(1) and LALR(1) parsing mechanisms.

**File:** `string_parser.py`

```python
# Example Usage
# string_parser.parse_string("ababc", clr1_parser_table)
# string_parser.parse_string("ababc", lalr1_parser_table)
```

## Observations and Conflicts

Please note that during the parsing process, any conflicts encountered will be pointed out in the console output. Conflicts may include shift-reduce or reduce-reduce conflicts, and they will be highlighted for further analysis.

Feel free to explore the code, run the scripts, and observe the parsing of the string "ababc" using CLR(1) and LALR(1) parsing mechanisms.

## Contributors

- [Zunysha Naveed - 21-CS-75]()
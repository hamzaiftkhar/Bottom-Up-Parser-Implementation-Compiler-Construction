# First and Follow Set Calculator

This Python script calculates the First and Follow sets for a given context-free grammar. It takes user input for the number of terminals, non-terminals, starting symbol, and productions. The script then displays the calculated First and Follow sets for each non-terminal.

## Requirements
- Python 3.x

## How to Use

1. Run the script by executing the following command in your terminal:

   ```bash
   python first_follow.py
   ```

2. Enter the required information when prompted:
   - Number of terminals
   - List of terminals
   - Number of non-terminals
   - List of non-terminals
   - Starting symbol
   - Number of productions
   - List of productions

3. The script will then display the calculated First and Follow sets for each non-terminal.

## Example

```bash
Enter no. of terminals: 3
Enter the terminals :
a
b
c
Enter no. of non terminals: 2
Enter the non terminals :
S
A
Enter the starting symbol: S
Enter no of productions: 2
Enter the productions:
S->aAb/c
A->bS/@
```

Output:

```
   Non Terminals           First               Follow       
         S            {'a', 'c', 'b'}           {'$', 'a', 'b'}
         A                  {'b', '@'}           {'$', 'a', 'b'}
```

## Notes
- The script uses recursion to calculate the First and Follow sets.
- "@" represents epsilon (empty string) in the Follow sets.

Feel free to use this script to analyze the grammar of your choice and understand its First and Follow sets.

## Contributer
- [Muahmmad Hasnain - 21-CS-96]()
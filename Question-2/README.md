# Parser Generator LR(0) and SLR(1)

## LR(0) Parser Generator

This C program is a simple parser generator that generates LR(0) parsing table and parses an input string based on a given context-free grammar. It utilizes closure-goto construction, first-follow set computation, and LR(0) parsing table creation to achieve its functionality.

## Table of Contents
- [Prerequisites](#prerequisites)
- [How to Use](#how-to-use)
- [File Descriptions](#file-descriptions)
- [Example](#example)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Ensure that you have the following installed on your system:

- GCC (GNU Compiler Collection)
- C Standard Library
- Make (optional but recommended for building)

## How to Use

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/parser-generator.git
   ```

2. Navigate to the project directory:

   ```bash
   cd parser-generator
   ```

3. Compile the program using GCC:

   ```bash
   make
   ```

   _If you don't have `make`, you can compile manually with:_

   ```bash
   gcc -o parser_generator main.c closure_goto.c parsingtable.c first_follow.c parse.c
   ```

4. Run the generated executable:

   ```bash
   ./parser_generator
   ```

5. The program will compute closures, gotos, first-follow sets, and create an LR(0) parsing table. Finally, it will parse the input string.

## File Descriptions

- `main.c`: The main driver program that coordinates the entire process.
- `closure_goto.h` and `closure_goto.c`: Implements the closure-goto construction.
- `parsingtable.h` and `parsingtable.c`: Creates the LR(0) parsing table.
- `first_follow.h` and `first_follow.c`: Computes the first-follow sets.
- `parse.h` and `parse.c`: Parses the input string based on the generated parsing table.

## Example

```c
#include<stdio.h>
#include<stdlib.h>
#include<string.h>

#include"closure_goto.h"
#include"parsingtable.h"
#include"first_follow.h"
#include"parse.h"

int main() {
	start();	//Compute closure and goto.

	initialize_first_follow();
	compute_first();
	compute_follow();

	create_parsing_table();

	parse();	//Parse the input string.

	return 0;
}
```

## Contributing

- [Muhammad Hasnain - 21-CS-45]()
- [Hamza Iftikhar - 21-CS-45]()

If you'd like to contribute to this project, please follow the [Contributing Guidelines](CONTRIBUTING.md).
# Delta-Space-Demonstration
# Delta Space 0.5 Programming Language Guide  

## Introduction  
Delta Space 0.5 is a simple interpreted programming language with a simple syntax. This version (0.5) includes basic features for working with variables, strings, numbers, arrays, and mathematical operations.  

## Basic Commands  

### 1. Initialization  
- `attach Workspace` – enables the workspace (required for variable operations)  
- `attach Method` – enables methods for data manipulation  

### 2. Output  
- `type word:` – prints text (enter text after the command)  
- `type var:` – prints a variable's value  
- `type sentence:` – prints text followed by a variable's value  
- `type string method:` – applies a method to a string variable and prints the result  
- `type integer method:` – applies a method to an integer variable and prints the result  
- `type arr<all>:` – prints all elements of an array  
- `move next` – line break (`\n`)  
- `move far` – tabulation (`\t`)  
- `release` – terminates the program and displays all results  

### 3. Working with Variables  
- `make var(` – creates a variable:  
  - Specify type (`string` or `integer`)  
  - Enter variable name  
  - Enter value  
- `change var:` – modifies a variable's value  
- `change var to method:` – applies a method to a variable and updates its value  

### 4. Working with Arrays  
- `make arr(` – creates a string array  
- `change arr:` – modifies an array:  
  - `append` – adds an element to the end  
  - `appbegin` – adds an element to the beginning  

### 5. String Methods  
- `lengthof` – string length  
- `find` – substring search (returns position)  
- `rfind` – reverse substring search  

### 6. Mathematical Methods  
- `add` – addition  
- `minus` – subtraction  
- `multiply` – multiplication  
- `divide` – division  
- `iseven` – checks if a number is even  
- `sqrt` – square root  
- `degree` – exponentiation  
- `module` – absolute value  
- `roundm` – round up  
- `roundl` – round down  
- `logarithm` – natural logarithm  
- `logarithm 10` – base-10 logarithm  
- `sinus` – sine  
- `cosine` – cosine  
- `tangent` – tangent  

## Code Examples  

### Example 1: Simple Output  
```
1  attach Workspace  
2  type word:  
3       Hello, world!  
4  move next  
5  type word:  
6       This is Delta Space!  
7  release  
```  

### Example 2: Working with Variables  
```
1  attach Workspace  
2  make var(  
3       string  
4       name  
5       Alex  
6   )  
7  make var(  
8       integer  
9       age  
10      25  
11  )  
12  type sentence:  
13      My name is  
14      string  
15      name  
16  type sentence:  
17      I am  
18      integer  
19      age  
20  release  
```  

### Example 3: Math Operations  
```
1  attach Workspace  
2  attach Method  
3  make var(  
4       integer  
5       number  
6       10  
7   )  
8  change var to method:  
9       integer  
10      number  
11      add  
12      5  
13  type var:  
14      integer  
15      number  
16  release  
```  

### Example 4: Working with Arrays  
```
1  attach Workspace  
2  make arr(  
3       string  
4       fruits  
5   )  
6  change arr:  
7       string  
8       fruits  
9       append  
10      apple  
11  change arr:  
12      string  
13      fruits  
14      append  
15      banana  
16  type arr<all>:  
17      string  
18      fruits  
19  release  
```  

## Errors and Solutions  

- **Error L1**: Workspace not attached – run `attach Workspace`  
- **Error V1**: Invalid data type – use `string` or `integer`  
- **Error V2**: Variable already exists – choose a different name  
- **Error V3**: Variable not found – check the name  
- **Error M1**: Invalid string method – use `lengthof`, `find`, or `rfind`  
- **Error M2**: Invalid math method – check available methods  
- **Error A1**: Division by zero – change the divisor  
- **Error R1**: Array already exists  
- **Error R2**: Array not found  

## Conclusion  
Delta Space 0.5 provides basic programming capabilities with a simple, Russian-inspired syntax. Always enable `Workspace` before starting, and use `Method` for advanced operations. Ensure correct command syntax and data types when writing programs.

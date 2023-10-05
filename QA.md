# C Test: Questions and Answers

### 1. How would you code the following expression in the С programming language? 

*Assign value of the variable b to the variable a:* 

        a) a==b;
        b) a=b;
        c) b=a;
        d) a:=b;

### Answer: b) a = b;


### 2. How would you code the following expression? 

*Assign the value of five to the second item of the Myarray array*

    a) int [1] Myarray = "five";
    b) Myarray[1] = 5;
    c) Myarray[2] = "five";
    d) Myarray[2] = 5;

### Answer: b) Myarray[1] = 5;


### 3. How to code the following expression **If value of the variable index is greater than size, then we increment the count variable**?

    a) if (index>size) { count++; } 
    b) if (index<=”size") {count += 1;}
    c) if (index>=size) { ++count; }
    d) if (index>="size") {count = count + 1}

### Answer: a) if (index > size) { count++; }


### 4. What is the range of the unsigned int data type on the 32-bit platforms?

    a) from 0 to 255
    b) from -32768 to 32767
    c) from 0 to 65535
    d) from 0 to 4 294 967 295

### Answer d) from 0 to 4 294 967 295


### 5. Given an array int L[3][3] = { { 2, 3, 4 }, { 3, 4, 8 }, { 1, 0, 9 } };. What is the value of the item L[1][2]

    a) 2
    b) 3
    c) 4
    d) 8

### Answer: d) 8


### 6. What is called a function prototype?

    a) A function description including function name, return value type, parameter names and types
    b) A function description including function name, return value type, and parameter types
    c) A function name and return value type
    d) A function description including function name, return value type, parameter names and types, and function body

### Answer: b) A function description including function name, return value type, and parameter types


### 7. How to specify the new file creation for reading and writing mode for a stream in the C programming language?

    a) a+
    b) wb
    c) w+
    d) w+b

### Answer: c) w+


### 8. What function, described in the header file, reads a character string from a file?

    a) gets()
    b) fputs()
    c) fgets()
    d) fscanf()

### Answer: c) fgets()


### 9. What is the M array size after the following code execution?:

```
char M[ ]="\nGoodlive"
```

    a) 10
    b) 8
    c) 9
    d) Undefined

### Answer: a) 10


### 10. When is it necessary to use the return operation in a function body?

    a) Always
    b) When it is necessary that the function returns a value.
    c) When it is necessary to provide exit from the function in any place.
    d) When a return value type is specified, including the void type.

### Answer: b) When it is necessary that the function returns a value.


### 11. What is the C programming language keyword that is used for a structured data type declaration that has all the members starting from the same address in memory.

    a) struct
    b) union
    c) enum
    d) template

### Answer: b) union


### 12. The C programming language logical expressions return the result of type

    a) integer
    b) boolean
    c) char
    d) logical

### Answer: b) boolean


### 13. Choose the correct variant of the C programming language expression for the condition of: **x belongs to the interval [0;10)**.

    a) x>=0; x<10                        
    b) 0<=x<10
    c) (x>0 && (x<=10)                
    d) (x>=0) && (x<10)

### Answer: d) (x>=0) && (x<10)


### 14. Select the group, containing a correctly written C programming language relation operator sequence
    a) ~ >, <, =, ?                        
    b) =, <>, ><, >
    c) ==, >=, <=, !=        
    d) ~ =>,=<, =, <

### Answer: c) ==, >=, <=, !=    

    
### 15. The body of which cycle will be executed at least once independently of the loop condition:

    a) while
    b) do while
    c) for
    d) there are no such cycle operators in C

### Answer: b) do while

    
### 16. What is the result of the following code execution 

```
int i=2;
switch (i) {
  case 1: i += 2;
  case 2: i *= 3;
  case 6: i /= 2;
  default: ;
}
```

    a) variable i gets the value of 6
    b) variable i gets the value of 3
    c) variable i gets the value of 2
    d) the switch operator body does not change the i variable value


### Answer: b) variable i gets the value of 3


### 17. Write a standard macro MIN that takes two arguments and returns the smallest of them.

### Answer:

```
#define MIN(x,y) ( ((x<y)*x) + ((y<x)*y) )
```

### 18. How to implement an infinite loop?

### Answer:

```
while(true) {
    // loop body goes here
}

```


### 19. Using the variable name *a*, write declaration for *a*:

#### (а) integer number

#### Answer (19.a):
```
int a;
```


#### (b) pointer to an integer number

#### Answer (19.b):

```
int* a;
```


#### (с) pointer to a pointer to an integer number

#### Answer (19.c):

```
int** a;
```


#### (d) array of ten integer numbers

#### Answer (19.d):

```
int a[10];
```


#### (е) array of ten pointers to integer numbers

#### Answer (19.e):

```
int* a[10];
```


#### (f)  pointer to an array of ten integer numbers

#### Answer: (19.f)

```
int arr[10];
int* a = arr;
```


#### (g) pointer to a function that receives an integer argument and returns an integer value

#### Answer (19.g):

```
int fn(int x) {
    return x;
}

int (*a)(int) = &fn;
```

### 20. For the given variable *a* write two code fragments. The first code fragment should set the third bit of that variable. The second one should clear the third bit of that variable. In both the cases, the other bits should remain unchanged.

### Definitions:
- setting the third bit means setting the value of the third bit to 1;
- clearing the third bit means setting the value of the third bit to 0;

### Order of bits: I'm counting the bits right to left:

```
01001011 : binary number
87654321 : bit count
```

I'm going to manipulate the bit at the position three as per *Order of bits* schema.
The code is written for char type variables.


### Answer:

```
void set_third_bit_to_one(char &value) {
    value = value | 4;
}

void set_third_bit_to_zero(char &value) {
    value = value & (~4);
}

```

### 21. Is the following code valid, and what does it perform?

```
int a = 5, b = 7, c;
c = a+++b;

```

### Answer: Yes, the code is valid. 

In the first line of the code: three integer variables are declared: a=5, b=7, and c.

In the second line of code a(5) added to b(7), the result of this operation is saved to c(12), and then post-increment applied to a(6).
 
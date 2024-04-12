# 1º Part - Go Program to Find Numbers Divisible by 3 between 1 and 100

The following Go program uses the % operator and a for loop to find and print all numbers between 1 and 100 that are divisible by 3:

```go
package main

import "fmt"

func main() {
  for i := 1; i <= 100; i++ {
    if i%3 == 0 {
      fmt.Println(i)
    }
  }
}
```

## Explanation:

- Importing fmt package: The line import "fmt" imports the fmt package, which provides functions for text formatting and printing.

- For loop: The for loop iterates from 1 to 100, assigning each value to the variable i.

- Divisibility check: The condition i%3 == 0 checks if the current value of i is divisible by 3 using the modulo operator %.

- Printing: If the condition is true, the value of i (a number divisible by 3) is printed to the console using the fmt.Println function.

# 2º Part - Go Program for "Pin-Pan" between 1 and 100

The following Go program implements the "Pin-Pan" game between 1 and 100, printing numbers or the words "Pin" and "Pan" according to the rules:

```go
package main

import "fmt"

func main() {
  for i := 1; i <= 100; i++ {
    if i%3 == 0 && i%5 == 0 {
      fmt.Println("Pin-Pan")
    } else if i%3 == 0 {
      fmt.Println("Pin")
    } else if i%5 == 0 {
      fmt.Println("Pan")
    } else {
      fmt.Println(i)
    }
  }
}
```

## Explanation:

Importing fmt package: The line import "fmt" imports the fmt package, which provides functions for text formatting and printing.

For loop: The for loop iterates from 1 to 100, assigning each value to the variable i.

Divisibility checks:

- The condition i%3 == 0 && i%5 == 0 checks if the current value of i is divisible by both 3 and 5 simultaneously. In this case, the word "Pin-Pan" is printed.
- The condition i%3 == 0 checks if the current value of i is divisible by 3. In this case, the word "Pin" is printed.
- The condition i%5 == 0 checks if the current value of i is divisible by 5. In this case, the word "Pan" is printed.
- Printing the number: If none of the above conditions are true, the value of i (a number that is not a multiple of 3 or 5) is printed to the console using the fmt.Println function.

This program implements the "Pin-Pan" game more comprehensively, using multiple divisibility checks and printing the words "Pin", "Pan", or the original number according to the rules.

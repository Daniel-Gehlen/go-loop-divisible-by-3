# Go Program to Find Numbers Divisible by 3 between 1 and 100

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

## Explanation:

- Importing fmt package: The line import "fmt" imports the fmt package, which provides functions for text formatting and printing.

- For loop: The for loop iterates from 1 to 100, assigning each value to the variable i.

- Divisibility check: The condition i%3 == 0 checks if the current value of i is divisible by 3 using the modulo operator %.

- Printing: If the condition is true, the value of i (a number divisible by 3) is printed to the console using the fmt.Println function.

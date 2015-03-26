# English3Java
The open source alternative to English2Java. Note that English3Java is still in the early stages of development and error handling is very minimal. We also recognize that it is not currently practical to use for any task of reasonable size or complexity, and aim to add features to change this.
## How to Use
Run with `ruby e3j.rb english.txt JavaClass`. This will read the English from `english.txt` and output the Java to `JavaClass.java`. To run the Java produced, run `javac JavaClass.java` and `java JavaClass`.
## Feature List
#### Commands
* `define x as y` -> `int x = y`, `String x = y`, or `boolean x = y`
* `set x to y` -> `x = y`
* `print x` -> `System.out.println(x)`
* `negate x` -> `x = !x`
* `increment x` -> `x++`
* `decrement x` -> `x--`
* `input string x` -> `String x = new java.util.Scanner(System.in).nextLine()`
* `input number x` -> `int x = new java.util.Scanner(System.in).nextLine()`
* `add y to x` -> `x += y`
* `subtract y from x` -> `x -= y`
* `multiply x by y` -> `x *= y`
* `divide x by y` -> `x /= y`
* `if condition ... end` -> `if(condition) { ... }`
* `unless condition ... end` -> `if(!condition) { ... }`
* `while condition ... end` -> `while(condition) { ... }`
* `until condition ... end` -> `while(!condition) { ... }`

#### Conditions
* `x` -> `x` for booleans
* `x equals y` -> `x == y` or `x.equals(y)`
* `x is less than y` -> `x < y`
* `x is greater than y` -> `x > y`
* `y divides x` -> `x % y == 0`
* `x and y` -> `x && y`
* `x or y` -> `x || y`
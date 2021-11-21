# Racket

## Basics
### Syntax & Semantics
Racket uses prefix notation where the operation is prior to the operands.
Statements must be encapsalated within cirular brackets ().
```Racket
(+1 2)
```
#### Variables
Variables are created by using the keyword define, variables can be made up of primitive datatypes, functions, or structs.
Primitive data types are mutable:
```Racket
99         ; integers
#b101      ; binary => 5
#x111      ; hex => 273
```
#### Operators
Contains the basic arithmatic functions:
\+  \-  \*  \/

expt          => exponent

quotient      => quotient

remainder     => aka modular division

exact-inexact => Goes from fractional form to decimal form.

##### Boolean operators:
not, and, or
#### String operators of interest:
string-append => appends two strings

string-ref    => refer to an index within a string

format        => insert strings into the first using the term ~a
```Racket
(format "~a name is ~a" "His" "Bobby"); => "His name is Bobby"
```
printf        => print a string
#### Functions

### Built in Data Structures
Racket has many built in data structures for programmers to take advantage of, however many have perks or drawbacks which need to be considered when using them.


#### Pairs
To create a pair use the keyword "cons". Structure which contains two values.
- To reference the first value use keywork "car"
- To reference the second value use keyowrk "cdr"

#### Lists
Lists are created with the keywork "list" or a single quote. Made from a recursively defined pair, which is in the form of a linked list:
\'(Pair1Value RemainderOfList(pair2Value RemainderOfList(Pair3Value RemainderOfList(Pair4Value NULL))))
Has linear accessing time
- The Keyword "car" still references the first value
- The keyword "cdr" references all values after the first value
- The keyword "cons" will add the new value to the start of the list
- The keyword "append" will append two lists to each other
```Racket
(define myList '("this" "Is" "My" "List"))
(car myList);                             => "this"
(cdr myList);                             => '("Is" "My" "List")
(cons "Hello" myList);                    => '("Hello" "This" "Is" "My" "List")
(append myList '("Anyways," "Goodbye"));  => '("this" "Is" "My" "List" "Anyways," "Goodbye")
```
<details>
<summary>Sources</summary>
https://docs.racket-lang.org/reference/pairs.html
</details>

#### Vector
fixed length arrays using \#

has constant time accessing of indecies.

```Racket
(define (ObjectsColliding(o1 o2))
(equal? o1 o2)
)
(define player (vector 1 3 3))
(define wall (vector 1 3 3))
ObjectsColliding(player wall))
)
```

<details>
<summary>Sources</summary>
https://docs.racket-lang.org/rosette-guide/sec_vec.html
https://docs.racket-lang.org/reference/vectors.html
https://learnxinyminutes.com/docs/racket/
</details>


#### Maps / Dictionaries / Hashes
Racket has the data structure Hashes built in, where hashes are a map of keys to values.
Accesses values in constant time for both muttable and immutable maps.

<details>
<summary>Sources</summary>
  https://learnxinyminutes.com/docs/racket/
https://docs.racket-lang.org/reference/hashtables.html
</details>
#### Sets

#### Structs
Structs are be default immutable, this can be changed by adding the "#:mutable" tag:
```Racket
(struct car(Make Model Year Color Mileage) #:mutable)
(define MyCar
  (car "Hyundai" "Elantra" "Gray" 117000)
)
```
### Under the hood

### Supported Paradigms 
#### Object Oriented Programming
Racket allows for the creation of objects and 

### Sources
https://learnxinyminutes.com/docs/racket/

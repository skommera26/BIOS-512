08/19/2025

Quotations:
- single quotations when printing somthing out
- Quotations evaluate to a string
- Set of characters between the "" evaluate to a string

  ```r
  "abcd"
  "10" # is a string
  10 # is an integer
  ```

  - Another way to have quotation marks in strings use this:
  ```r
  "This includes quotes:\"\""
  "This includes backslashes:\\""
  ```
  - Use backslashes to include quotes

Variables
  - Use assignment opperators to assign variable a charater/ number/ anything
  - can use:
    - <-
    - =
    - <<-: used to change a varibale completed and update it; look for closest bidning and change it; used to change global variable;
      - go up until you find something and change it there 


Loops + For  in
- While loops: undetermined number of times to do something until a condition is true
- For loops: loops exactly the same number of times we have element sin the vector
    - @ end of code, x is equal to last element in vector 


Functions
- c, +, - are functions, but they are primative funcitons: built-in function calls

```r
`+` # will run back to the last way we can backtrack so it will say .Primitive("+") bc cant backtrack any furtehr
```
- Everytime a fucntion is called a new environment is created
- can create your own funciton using function() argument

```r
quadratic_formula <- function(a,b,c) {
  r <- sqrt(b*b - 4*a*c);
  n1 <- -b + r;
  n2 <- -b-r;
  d <- 2*a;
  c(n1/d, n2/d);
}

quadratic_formula(9,100,11)
c(r,n1,n2,d)
```

** notice w curley brakeys they open in that line of code, and you press enter to start code within curly brackt on other line
** you end the code with the curly braket on a seperate line

```r
make_counter <- function(start, incr){
    value <- start;
    function(){
        old_value <- value;
        value <<- value + incr; ## Update the old value in the parent scope.
        # having <<- instead of <- helps update the value rather than keep it the same like <- would do
        old_value;
    }
}
counter_from_1 <- make_counter(1,1);
counter_from_1()
counter_from_1()
```







  

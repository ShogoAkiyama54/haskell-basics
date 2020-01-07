# haskell-basics
Basic Haskell syntax and examples learned through [Learn You a Haskell for Great Good](http://learnyouahaskell.com/)

## How to complie and run Haskell code
I use GHC as the book does. Download the Haskell Platform through [here](https://www.haskell.org/platform/).

+ start the interactive mode of GHC: `ghci` at the prompt. 
+ load a haskell file: `:l functions` where the file name is *functions.hs*
+ reload the current script: `:r`

## Reserved Words
+ `let` can be used to define a name in GHCI. Doing `let a = 1` inside GHCI is the equivalent of writing `a = 1` in a script and then loading it. 

## Boolean Algebra
+ `&&` means *and*
+ `||` means *or*
+ `not` negates a `True` or `False` 

## Testing for Equality
+ `==` means *equal*
+ `/=` means *unequal* 

but they can compare only the same type

## Built-in Functions
+ `succ` A: takes anything that has a defined successor and returns that successor. 
+ `min` A B: takes two things that can be put in an order and returns the lesser one.
+ `max` A B: takes two things that can be put in an order and returns the greater one.

## Build-in Functions for List Operations
+ `++`: puts two list together 
```
[1,2,3,4] ++ [9,10,11,12]
>[1,2,3,4,9,10,11,12]
```
+ `:`: 

## String in Haskell
string type in Haskell is just a list of character. That is, `"hello"` is just syntax suger for `['h','e','l','l','o']`.

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
+ `[A] ++ [B]`: puts two list together. Haskell goes through the whole elements of the left side list to append the right list.
```
ghci> [1,2,3,4] ++ [9,10,11,12]
[1,2,3,4,9,10,11,12]
```
+ `A : [B]`: puts an element to the head of the list
```
ghci> 'A' : " SMALL CAT"
"A SMALL CAT"
```
+ `[A] !! B`: takes an element out of the a list by index. The indices start at 0.
```
ghci> "Steve Buscemi" !! 6
'B'
```
+ `head [A]`: takes a list and returns its head.
```
ghci> head [5,4,3,2,1]
5
```
+ `tail [A]`: takes a list and returns its tail. In other words, it chops off a list's head.
```
ghci> tail [5,4,3,2,1]
[4,3,2,1]
```
+ `last [A]`: takes a list and returns its last element.
```
ghci> last [5,4,3,2,1]
1
```
+ `init [A]`: takes a list and returns everything except its last element.
```
ghci> init [5,4,3,2,1]
[5,4,3,2]
```
`head`, `tail`, `last`, and `init` will throw an exception when used on empty lists.

+ `length [A]`: takes a list and returns its length.
```
ghci> length [5,4,3,2,1]
5
```
+ `null [A]`: checks if a list is empty. If it is, it returns True, otherwise it returns False. Use this function instead of xs == [] (if you have a list called xs)
```
ghci> null [1,2,3]
False
ghci> null []
True
```

## List in Haskell
`[1,2,3]` is actually just syntactic sugar for `1:2:3:[]`. `[]` is an empty list.

## String in Haskell
string type in Haskell is just a list of character. That is, `"hello"` is just syntax suger for `['h','e','l','l','o']`.

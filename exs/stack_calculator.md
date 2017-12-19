# Stack calculator

## Context

Your great, precious, marvellous calculator broke down !
What a shame !
But instead of borrowing your friend's calculator (if you have any) or to buy a new one or even to use your goddamn phone, you chose the one, _true_ way.
The way of the [stack](https://en.wikipedia.org/wiki/Stack_%28abstract_data_type%29) !

## Summary

Your program must be able to calculate from a [stack](https://en.wikipedia.org/wiki/Stack_%28abstract_data_type%29) any data type (or close to any).

Supported data types:
- int
- float
- string

| Command | Description |
|---------|-------------|
| `push <variable> [...]` | Push N variables into the stack |
| `add` | Add first 2 variables of the stack. Push the result into the stack |
| `sub` | Substract first 2 variables of the stack. Push the result into the stack |
| `div` | Divide first 2 variables of the stack. Push the result into the stack |
| `mul` | Multiply first 2 variables of the stack. Push the result into the stack |
| `pop` | Pop the first variable from the stack |
| `clear` | Remove every variable from the stack |

Commands must be non [case-sensitive](https://en.wikipedia.org/wiki/Case_sensitivity)


The following operations are permitted:

| Variable N | Operation | Variable N+1 | Result | Example |
|------------|-----------|--------------|--------|---------|
| int | add, sub, div, mul | int | int | 1 add 1: 2 |
| int | add, sub, div, mul | float | float | 1 add 1.1: 2.1 |
| int | add | string | string | 1 add "hello": "1hello" |
| int | mul | string | string | 2 mul "hello": "hellohello" |
| float | add, sub, div, mul | float | float | 1.1 add 1.1: 2.2 |
| float | add | string | string | 42.2 add "hello": "42.2hello" |
| string | add | string | string | "hello" add "world": "helloworld" |

## Example

```
./stack_calculator
> push 41
> push 1
> add
> dump
< [ 42 ]
> push 0.1
> dump
< [ 0.1, 42 ]
> add
< [ 42.1 ]
> pop
> dump
> [ ]

./stack_calculator
> hello
< Unknown command: "hello"
> add
< Not enough variable on stack
> push 1 2
> dump
< [ 2, 1 ]
> sub
> dump
< [ 1 ]
> clear
> dump
< [ ]

./stack_calculator
> push 42 "Je suis un chat !"
> add
> dump
< [ "42Je suis un chat" ]
> clear
> push "abc" 3
> sub
< Operation not permitted
> mul
> dump
< [ "abcabcabc" ]
```

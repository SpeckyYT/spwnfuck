# SPWNFuck

Run BrainFuck code directly from SPWN 😎

## How?

```rs
import spwnfuck

output = @brainfuck::new(
    instructions = ">++++++++[-<++++++++>]<+++++.", // brainfuck code
    length = 10, // memory length limit [*]
    bits = 8, // memory size limit
    timeout = 10, // timeout in seconds [*]
    input = [], // input for , operators [*]
    native = true, // compiles the bf code to spwn and runs it
)

// [*] doesn't do anything if `native` is on

$.print(output)
```

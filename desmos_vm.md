ie: dvm
stacked based bytecode vm
each instruction is split into three numbers:
    first is the op
    second is the operand
instruction/data array and stack
instruction pointer and stack pointer
Instructions:

pus: push next instruction to stack and increment instruction pointer
pop: pop top val from stack (could also do w/ instruction pointer)

add: add the top two values of the stack, popping them in the process, and add new value to top of stack
sub: sub the top two values of the stack, popping them in the process, and add new value to top of stack
mul: mul the top two values of the stack, popping them in the process, and add new value to top of stack
div: div the top two values of the stack, popping them in the process, and add new value to top of stack
out: print the top value of the stack and pop it
inp: read input and push it to the stack
jeq: jump to ip x if the instruction pointer is equal to 0



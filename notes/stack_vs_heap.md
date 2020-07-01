## Stack

- Fills in from top to bottom (backwards from high memory to low memory)
- Only exists in a function
- Once function is exited the pointer to that thing might point to a 
new thing that has overwritten that location in memory...
- going to have large values

## Heap

- If memory is needed for long
- need to use `new` keyword. `new`:
	1. Allocates memory in heap for data structure
	1. Initialises the data structure
	1. Returns a pointer to the start of the data structure
- memory is only reclaimed once pointer is passed to `delete` operator
- Before we do anything with heap it is just what is laying around from 
the operating system.
- going to have small values and grow up

## Null pointers

- once we delete something in heap memory, you are still left with 
the pointer. Therfore to delete something from heap memory completely
you can `  delete c;  c = nullptr;`. `nullptr` points to the memory 
address **0x0**
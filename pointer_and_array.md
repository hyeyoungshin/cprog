# Pointer and array

In C, whenever we use &var_name[0] we can replace that with var_name.

`ptr = &my_array[0];`
`ptr = my_array;`


The name of the array is the address of first element in the array. For example, while we can write

`ptr = my_array;`

we cannot write

`my_array = ptr;`


The reason is that while **ptr** is a variable **my_array** is a constant. That is, the location at which the first element of **my_array** will be stored cannot be changed once **my_array[]** has been declared.

"An **object** is a named region of storage; an **lvalue** is an expression referring to an object".

Since **my_array** is a named region of storae, why is **my_array** in the above assignment statement not an **lvalue**? To resolve this problem, we refer to **my_array** as an "unmodifiable lvalue".


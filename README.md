\_printf

\_printf is a custom implementation of the C programming function printf. This project is an application of the C programming knowledge.

Prototype: int \_printf(const char \*format, ...);

Project Requirements

Code must follow the Betty style

Global variables are not allowed

Authorized functions and macros:

write (man 2 write)

malloc (man 3 malloc)

free (man 3 free)

va_start (man 3 va_start)

va_end (man 3 va_end)

va_copy (man 3 va_copy)

va_arg (man 3 va_arg)

Mandatory Tasks

0- Write function that produces output with conversion specifiers c, s, and %.

1- Handle conversion specifiers d, i.

2- Create a man page for your function.

Advanced Tasks

3- Handle conversion specifier b.

4- Handle conversion specifiers u, o, x, X.

5- Use a local buffer of 1024 chars in order to call write as little as possible.

6- Handle conversion specifier S.

7- Handle conversion specifier p.

8- Handle flag characters +, space, and # for non-custom conversion specifiers.

9- Handle length modifiers l and h for non-custom conversion specifiers.

10- Handle the field width for non-custom conversion specifiers.

11- Handle the precision for non-custom conversion specifiers.

12- Handle the 0 flag character for non-custom conversion specifiers.

13- Handle the custom conversion specifier r that prints the reversed string.

15- Handle the custom conversion specifier R that prints the rot13'ed string.

16- All above options should work well together.

File Descriptions

\_printf.c

contains the fucntion \_printf, which uses the prototype int \_printf(const char \*format, ...);. The format string is composed of zero or more directives. See man 3 printf for more detail. \_printf will return the number of characters printed (excluding the null byte used to end output to strings) and will write output to stdout, the standard output stream.

\_putchar.c

contains the function \_putchar, which writes a character to stdout. main.h \*contains all function prototypes used for \_printf.

man_3_printf

manual page for the custom \_printf function.

functions.c functions1.c functions2.c

contains all function of each specifier used for \_printf. all function have its own description inside the file.

handle_print.c

contains arguments types used for \_printf.

get_flags.c

contains all function for each flag use for \_printf.

utils.c

contains some necessary functionalities for \_printf.

get_width.c

contains functions to get width for spcifics spcifiers.

write_handlers.c

contains write functions.

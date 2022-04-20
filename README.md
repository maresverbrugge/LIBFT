# LIBFT

## AIM:
This project allows you to re-write the highly useful standars functions. You'll understand them better,
and learn to use them. This library will be helpful with all your future C projects.

![](libft.png)

## FUNCTIONS:
**Part 1:**

◦ [isalpha()](libft/ft_isalpha.c): this function tests for any character for which isupper() or islower() is true.

◦ [isdigit()](libft/ft_isdigit.c): this function tests for a decimal digit character.

◦ [isalnum()](libft/ft_isalnum.c): this function tests for any character for which isalpha() or isdigit() is true.

◦ isascii(): this function tests for an ASCII character, which is any character between 0 and octal 0177 inclusive.

◦ isprint(): this function tests for any printing character, including space (` ').

◦ strlen(): this function computes the length of the string s.

◦ memset(): this function writes len bytes of value c (converted to an unsigned char) to the string b.

◦ bzero(): this function writes n zeroed bytes to the string s. If n is zero, bzero() does nothing.

◦ memcpy(): this function copies n bytes from memory area src to memory area dst.

◦ memccpy() this function copies bytes from string src to string dst. If the character c occurs in the string src, the copy stops and a pointer to the byte after the copy of c in the string dst is returned.

◦ memmove(): this function copies len bytes from string src to string dst.

◦ strlcpy(): this function copies and concatenates strings.*

◦ strlcat(): this function copies and concatenates strings.* 

◦ toupper(): this function converts a lower-case letter to the corresponding upper-case letter.

◦ tolower(): this function converts an upper-case letter to the corresponding lower-case letter.

◦ strchr(): this function locates the first occurrence of c (converted to a char) in the string pointed to by s.

◦ strrchr(): this function locates the last occurrence of c (converted to a char) in the string pointed to by s.

◦ strncmp(): this function lexicographically compares the null-terminated strings s1 and s2, comparing not more than n characters.

◦ memchr(): this function locates the first occurrence of c (converted to an unsigned char) in string s.

◦ memcmp(): this function compares byte string s1 against byte string s2.

◦ strnstr(): this function locates the first occurrence of the null-terminated string needle in the string haystack, where not more than len characters are searched.

◦ atoi(): this function converts the initial portion of the string pointed to by str to int representation.

◦ calloc(): this function contiguously allocates enough space for count objects that are size bytes of memory each and returns a pointer to the allocated memory. The allocated memory is filled with bytes of value zero.

◦ strdup(): this function allocates sufficient memory for a copy of the string s1, does the copy, and returns a pointer to it. The pointer may subsequently be used as an argument to the function free().

**Part 2:**

◦ substr(): allocates (with malloc) and returns a substring from the string ’s’. The substring begins at index ’start’ and is of maximum size ’len’.

◦ strjoin(): allocates (with malloc) and returns a new string, which is the result of the concatenation of ’s1’ and ’s2’.

◦ strtrim(): allocates (with malloc) and returns a copy of ’s1’ with the characters specified in ’set’ removed from the beginning and the end of the string.

◦ split(): allocates (with malloc) and returns an array of strings obtained by splitting ’s’ using the character ’c’ as a delimiter.

◦ itoa(): allocates (with malloc) and returns a string representing the integer received as an argument. Negative numbers must be handled.

◦ strmapi(): applies the function ’f’ to each character of the string ’s’ to create anew string (with malloc) resulting from successive applications of ’f’.

◦ put_char_fd(): outputs the character ’c’ to the given file descriptor.

◦ put_str_fd(): outputs the string ’s’ to the given file descriptor.

◦ put_endl_fd(): outputs the string ’s’ to the given file descriptor, followed by a newline.

◦ put_nbr_fd(): outputs the integer ’n’ to the given file descriptor.

*check man pages to discover the difference between strlcpy en strlcat!


**Bonus:**

The bonus makes you work with a lists of structs. 

◦ lst_new(): allocates (malloc) and returns a new element. The variable ’content’ is initialized with the value of the parameter ’content’. The variable ’next’ is initialized to NULL.

◦ lst_add_front(): adds the element ’new’ at the beginning of the list.

◦ lst_size(): counts the number of elements in a list.

◦ lst_last(): returns the last element of the list

◦ lst_add_back(): adds the element 'new' at the end of the list.

◦ lst_delone(): takes as a parameter an element and frees the memory of the element’s content using the function ’del’ given as a parameter and free the element. The memory of ’next’ must not be freed.

◦ lst_clear(): deletes and frees the given element and every successor of that element, using the function ’del’ and free(). Finally, the pointer to the list must be set to NULL.

◦ lst_iter(): iterates the list ’lst’ and applies the function ’f’ to the content of each element.


## TECHNICAL:

◦ The function names have the following structure: ft_LibraryFuctionName. (In case you're like me and only find out after months: "ft" stands for forty-two. Yes, 42.)

◦ All function are compiled with the following flags: -Wall -Wextra -Werror.

◦ Allowed functions: malloc, free, write

## USAGE:

After cloning this repo, you can create the library libft.a by running "make" in the command line. Running "make bonus" will also compile the library with the bonus functions.

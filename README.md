
# 💠 **LIBFT** 

> _`libft` is the first project in the School 42 common core curriculum, aimed at developing a custom C library._

----------

## 📋 **Table of Contents** 

1.  [Introduction](#introduction)
2.  [Project Subject](#project-subject)
3.  [Documentation](#documentation)
4.  [How to Use/Test](#how-to-usetest)
5.  [References](#references)
6.  [Evaluation](#evaluation)

----------

## 📍 **Introduction**

The objective is to implement a range of general-purpose functions that are commonly available in standard libraries, as well as additional functions designed by the developer. <br> <br>
This project focuses on creating a comprehensive library of utilities that will be fundamental for various programming tasks. It serves as a foundational exercise in C programming, providing essential functions to support future projects.

----------

##  📚 **Project Subject**

### Table

| Attribute            | Details                                                                                           |
|----------------------|---------------------------------------------------------------------------------------------------|
| Program Name         | `libft`                                                                                           |
| Turn In Files        | `libft.h`, `*.c` files                                                                           |
| Makefile             | `Makefile`                                                                                       |
| External Functions   | None                                                                                              |
| Libft Authorized     | N/A                                                                                           |
| Description          | Development of a custom C library containing general-purpose functions and additional utilities. |

### Subject PDF

For more details about the project subject, refer to the [Subject PDF](link_to_subject_pdf).

### Advice 📝

- **Norminette**: Ensure that all code adheres to the coding standards enforced by Norminette. This includes formatting, function length, variable naming, and overall code style. Failure to comply with these standards will result in code rejection.
  
- **Memory Leaks**: Verify that the project does not produce memory leaks. Use tools such as Valgrind to check for any memory allocation issues and ensure that all dynamically allocated memory is properly freed.

- **Segmentation Faults**: Thoroughly test the code to prevent segmentation faults. Make sure all pointers are properly initialized and that memory accesses are within valid bounds.

- **Flags Used**: Utilize appropriate compiler flags for debugging and optimization. For example, use `-Wall -Wextra -Werror` to enable all warnings and treat them as errors. Ensure that the Makefile includes commands to compile with these flags to maintain code quality.

- **Testing**: Implement comprehensive testing for all functions to verify correctness and robustness. Ensure that tests cover various edge cases and typical usage scenarios.

----------

## 📄 **Documentation**

For a comprehensive overview of the project, including detailed explanations of how the program is implemented and additional coding insights, please visit the Notion page linked below. This documentation provides an in-depth look at the project's design, structure, and functionality.

Access the full documentation here

### Functions Overview

| **Function Name** | **Description**                                                                                                                                                           |
|-------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `ft_isalpha`      | Checks if the character is an alphabetic letter.                                                                                                                             |
| `ft_isdigit`      | Checks if the character is a digit.                                                                                                                                           |
| `ft_isalnum`      | Checks if the character is alphanumeric (i.e., a letter or a digit).                                                                                                        |
| `ft_isascii`      | Checks if the character is an ASCII character.                                                                                                                               |
| `ft_isprint`      | Checks if the character is printable (including space).                                                                                                                       |
| `ft_strlen`       | Computes the length of a string (excluding the null terminator).                                                                                                             |
| `ft_memset`       | Fills the first `n` bytes of the memory area with the constant byte `c`.                                                                                                    |
| `ft_bzero`        | Sets the first `n` bytes of the memory area to zero.                                                                                                                         |
| `ft_memcpy`       | Copies `n` bytes from one memory area to another.                                                                                                                            |
| `ft_memmove`      | Moves `n` bytes from one memory area to another, handling overlapping regions.                                                                                             |
| `ft_strlcpy`      | Copies up to `size - 1` characters from a string to another and null-terminates the destination.                                                                             |
| `ft_strlcat`      | Appends up to `size - strlen(dst) - 1` characters from a string to another and null-terminates the result.                                                                    |
| `ft_toupper`      | Converts a character to uppercase.                                                                                                                                             |
| `ft_tolower`      | Converts a character to lowercase.                                                                                                                                             |
| `ft_strchr`       | Locates the first occurrence of a character in a string.                                                                                                                     |
| `ft_strrchr`      | Locates the last occurrence of a character in a string.                                                                                                                      |
| `ft_strncmp`      | Compares up to `n` characters of two strings.                                                                                                                                |
| `ft_memchr`       | Locates the first occurrence of a byte in a memory block.                                                                                                                    |
| `ft_memcmp`       | Compares `n` bytes of two memory blocks.                                                                                                                                       |
| `ft_strnstr`      | Finds the first occurrence of a substring within a string, up to `len` characters.                                                                                          |
| `ft_atoi`         | Converts a string to an integer.                                                                                                                                              |
| `ft_calloc`       | Allocates memory for an array of `nmemb` elements of `size` bytes each and initializes all bytes to zero. Uses `malloc()`.                                                   |
| `ft_strdup`       | Duplicates a string by allocating sufficient memory and copying the string into the new memory area. Uses `malloc()`.                                                         |

### External Functions Overview

| **Function Name** | **Description**                                                                                              |
|-------------------|--------------------------------------------------------------------------------------------------------------|
| `ft_substr`       | Allocates (with `malloc(3)`) and returns a substring from the string `s`. The substring starts at `start` and has a maximum size of `len`. |
| `ft_strjoin`      | Allocates (with `malloc(3)`) and returns a new string that is the result of concatenating `s1` and `s2`.     |
| `ft_strtrim`      | Allocates (with `malloc(3)`) and returns a copy of `s1` with characters specified in `set` removed from both ends. |
| `ft_split`        | Allocates (with `malloc(3)`) and returns an array of strings split by the character `c`. The array ends with a NULL pointer. |
| `ft_itoa`         | Allocates (with `malloc(3)`) and returns a string representing the integer `n`. Handles negative numbers.    |
| `ft_strmapi`      | Applies function `f` to each character of `s`, creating a new string with results. Allocates memory with `malloc(3)`. |
| `ft_striteri`     | Applies function `f` to each character of `s`, modifying each character in place.                           |
| `ft_putchar_fd`   | Outputs character `c` to the file descriptor `fd`.                                                           |
| `ft_putstr_fd`    | Outputs the string `s` to the file descriptor `fd`.                                                          |
| `ft_putendl_fd`   | Outputs the string `s` to the file descriptor `fd` followed by a newline.                                    |
| `ft_putnbr_fd`    | Outputs the integer `n` to the file descriptor `fd`.                                                          |



----------

## 🛠️ **How to Use/Test** 

_Clear instructions on how to run the project, install dependencies, or run tests, if applicable._

Example:

### Installation

1.  Clone the repository:
    
 ### Execution

To run the project, use the command: `bash ./executable-name`

### Tests

To run the tests: `bash ./run_tests.sh`

----------

## 🔗 **References** 

_Links or citations of materials and resources used for the development of the project._

Example:

-   Official Documentation for Library X
-   Article on Algorithm Y

----------

## 🏆 **Evaluation** 

_Section where you can add the result of the project's evaluation, if available, and received feedback._

Example:  
"The project was evaluated with a score of X/100. Additional comments: `feedback from evaluators`."

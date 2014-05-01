## Files

### Character Encoding

PHP code MUST use only UTF-8 without BOM.

All PHP files MUST use the Unix LF (linefeed) line ending.

### PHP Tags

For reasons of portability, PHP code MUST use the long `<?php ?>` tags or the short-echo `<?= ?>` tags; it
MUST NOT use the other tag variations.

The closing `?>` tag MUST be omitted from files containing only PHP.

### Side Effects

The phrase "side effects" means execution of logic not directly related to declaring classes, functions, constants, etc., *merely from including the file*.

"Side effects" include but are not limited to: generating output, explicit use of `require` or `include`, connecting to external services, modifying ini settings, emitting errors or exceptions, modifying global or static variables, reading from or writing to a file, and so on.

A file SHOULD declare new symbols (classes, functions, constants, etc.) and cause no other side effects, or it SHOULD execute logic with side effects, but SHOULD NOT do both.

### Lines

There MUST NOT be more than one statement per line.

There MUST NOT be a hard limit on line length.

The soft limit on line length MUST be 120 characters; automated style checkers MUST warn but MUST NOT error at the soft limit.

Lines SHOULD NOT be longer than 80 characters; lines longer than that SHOULD be split into multiple subsequent lines of no more than 80 characters each.

There MUST NOT be trailing whitespace at the end of non-blank lines.

Blank lines MAY be added to improve readability and to indicate related blocks of code.

All PHP files MUST end with a single blank line.

### Indenting

Code MUST use an indent of 4 spaces, and MUST NOT use tabs for indenting.

Using proper tabs instead of spaces allows individual developers to set their own preferred level of indentation in their editor of choice. Spaces can then be used to insert fine-grained sub-indentation for inter-line alignment.
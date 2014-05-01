## Case, Naming and Brace Conventions

PHP [keywords](http://php.net/manual/en/reserved.keywords.php) MUST be in lower case.

All constants — both class and global — MUST be declared in all upper case with
underscore separators.

The PHP constants `true`, `false`, and `null` MUST be in lower case.

Class names MUST be declared in `StudlyCaps`.

Functions, method names and properties MUST be declared in `camelCase()`.

### Braces

Allman style MUST be used for class, method and function definitions; the 1TBS variant of K&R MUST be used in code bodies.

- Opening braces for definitions MUST go on the next line, and closing braces MUST go on the next line after the body.

### Control Structures

The [alternative syntax](http://php.net/manual/en/control-structures.alternative-syntax.php) for control structures SHOULD NOT be used.

The body of each structure MUST be enclosed by braces — even single liners. This standardizes how the structures look, and reduces the likelihood of introducing errors as new lines get added to the body.

The general style rules for control structures are as follows

- There MUST be one space after the control structure keyword
- There MUST NOT be a space after the opening parenthesis
- There MUST NOT be a space before the closing parenthesis
- There MUST be one space between the closing parenthesis and the opening brace; opening braces for control structures MUST go on the same line
- The structure body MUST be indented once
- The closing brace MUST be on the next line after the body.

### 5.1. `if`, `elseif`, `else`

Any `else` or `elseif` keywords SHOULD be on the same line as the closing brace from the earlier body.

The keyword `elseif` SHOULD be used instead of `else if` so that all control keywords are represented as single words.

### 5.2. `switch`, `case`

- The `case` statement MUST be indented once from `switch`
- The `break` keyword (or other terminating keyword) MUST be indented at the same level as the `case` body
- There SHOULD be an empty line after `break` keyword
- There MUST be a comment such as `// no break` when fall-through is intentional in a non-empty `case` body.
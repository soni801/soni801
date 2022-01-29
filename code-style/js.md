# JavaScript Code style

The key words “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”, “SHOULD NOT”, “RECOMMENDED”, “MAY”, and
“OPTIONAL” in this document are to be interpreted as described in [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt).

This is my preferred JavaScript code style for performance and readability. To contribute JavaScript code to any of my
projects, you MUST follow this code style:

### Capitalisation

- `camelCase` MUST be used for
  - Object names
  - Variable names
  - Function names
- `kebab-case` MUST be used for
  - File names

### Language

- Hungarian notation MUST NOT be used
- Any characters outside the english alphabet SHOULD NOT be used in code nor comments
  - Other characters MAY be used if it is crucial for the functionality of the project
- You MUST use en_US in both code and comments
  - e.g. *color* as opposed to *colour*
- Profanity MUST NOT be used unless crucial for the functionality of the project

### Code style

- Newlines MUST be used for
  - `{` where strictly necessary
    - e.g. after `function`, `if`
  - Continuation of previous statements
    - e.g. `else` or `catch`
- You MUST omit curly brackets (`{}`) where possible
  - When omitting, content MUST NOT be placed on newline
- Inline curly brackets (`{}`) SHOULD be used
  - For `const` where several objects are defined
  - When objects are passed along to a function or constructor
- Parentheses MUST be omitted
  - In arrow function expressions with only one argument
- A space MUST precede
  - The arrow operator (`=>`)
- A space MUST follow
  - `if`, `function`
  - `,` unless at the end of a line
- Spaces MUST surround
  - Logical operators
    - e.g. `==`, `!=`, `>=`, `<=`, `&&`, `||`
    - The negating operator `!` SHOULD NOT be surrounded by spaces
  - Arithmetic operators
    - e.g. `+`, `-`, `*`, `/`
    - Incremental operators (`++`, `--`) MUST NOT be surrounded by spaces
    - The inversion operator `-` MAY not have a trailing space
  - Declaration operators
    - e.g. `=`
  - Content of inline curly brackets (`{}`)
  - Ternary operators (`?`, `:`)
- Single-line comments MUST have a space after `//` unless the comment contains only valid code
- There MUST NOT be any trailing whitespace on any line
- Double quotes SHOULD be used
  - Singe quotes MAY be used to avoid escaping in-string characters
  - String literals SHOULD be used where one or more variable is mentioned in the string
- Semicolons MUST be used where possible
- `const` MUST be used where the value will not change
- `var` SHOULD NOT be used. `let` SHOULD be used instead
- You MUST use 4 spaces indentation
  - The Tab character MUST NOT be used
- Any logical statement MUST stay on one line.
  - e.g. ternary operators, arithmetic statements or declarations.
- Function calls MUST be on the same line as the object they are called on
  - This does not apply if the function calls are used solely to set different properties of an element
- Strings MUST contain no line breaks
  - This does not apply if the string must have a line break for its functionality

### Version control

- You MUST use [conventional commits](https://www.conventionalcommits.org/) types.
  - The rest of the *conventional commits* specification SHOULD be followed.
- Commit names MUST be `lowercase` only.
  - This does not apply when referring to code or other proper names.
- Commits MAY be gpg-signed.
- There SHOULD only be one action done per commit.
  - Large commits that make many changes SHOULD be split up into several smaller commits.
- A new branch SHOULD be created for every major change
  - The branch name SHOULD start with `feat/`, `fix/`, or any other relevant type from the *conventional commits*
specification.

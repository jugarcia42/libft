#NormalizePath

##Description

Normalize Path is a programming exercise that focuses on implementing Unix-style path normalization.

Given a string representing a file system path, the goal is to convert it into its canonical form by removing redundant elements such as current directory references, parent directory references, and duplicated slashes.

This type of problem is common in file systems, web routing, and operating systems.

## Normalization rules

A path may contain:

- `.` → current directory (ignored)
- `..` → parent directory (go one level up)
- `/` → directory separator
- multiple consecutive `/` → treated as a single separator

## Examples

### Example 1

```text
Input: /home//user/./docs
Output: /home/user/docs
```

### Example 2

```text
Input: /home/user/../docs
Output: /home/docs
```

### Example 3

```text
Input: /../
Output: /
```

### Example 4

```text
Input: /a/./b/../../c/
Output: /c
```

##Concepts covered

-Java programming
-String manipulation
- Stack usage
- Path parsing
- Edge case handling
- Algorithm design
- Filesystem modeling

##Solution strategy

A typical approach:

1. Split the path by `/`.
2. Iterate through each segment:
   - Ignore empty strings and `.`.
   - If `..`, pop from stack if possible.
   - Otherwise, push valid directory names.
3. Rebuild the normalized path from the stack.

## Edge cases

- Multiple consecutive slashes (`///a//b`)
- Going above root (`/../../`)
- Empty or root-equivalent paths
- Paths without leading slash

##Objective

The goal of this exercise is to practice:

- String parsing
- Stack data structure usage
- Edge case handling
- Hierarchical data normalization
- Robust algorithm design

##Author

Programming exercise implemented in Java as a practice of data structures and path manipulation.

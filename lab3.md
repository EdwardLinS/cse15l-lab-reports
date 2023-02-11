# Command: `grep`

- Choose command
- Four interesting cmd options
  - two examples using it on files and directories from ./written_2
    - use code blocks to show cmd and output
    - sentence about what it's doing and why it's useful
  - cite online source for each 
    
  - in total: 8 examples
  - 2 examples for each of the 4 cmd option
  
  
## 4 *grep* command options
- `grep -v` / `grep --invert-match`
  - **What:** This command option selects non-matching lines
  - **Why:** This is useful for finding files that don't have the specified pattern
  - *Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/*
- `grep -i` / `grep --ignore-case`
  - **What:** This command option matches without matching case
  - **Why:** This is useful when you are purely looking for the pattern and not caring about specific case of the pattern.
  - *Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/*
- `grep -c` / `grep --count`
  - **What:** This command option prints out count of matching lines instead of normal grep output
  - **Why:** This is useful when the count of files is necessary and not file path or content.
  - *Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/*
- `grep -r` / `grep --recursive`
  - **What:** This command option greps all files in each directory recursively
  - **Why:** This is useful to grep all the files inside a directory with many different directories inside it. It removes the need to go through each directory.
  - *Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/*
- `grep -l` / `grep --files-with-matches` 
  - **What:** This command option prints the name of the file that has the match
  - **Why:** This is useful when only the path or name of the file is needed.
  - *Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/*

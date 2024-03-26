#Day2 - Linux Command Notes

1. **cp (Copy)**
   - **Syntax:** `cp [options] source destination`
   - **Function:** Copies files and directories from a source location to a destination location.
   - **Options:**
     - `-r`: Copies directories recursively.
     - `-i`: Prompts before overwriting existing files.
     - `-v`: Verbose mode, shows files as they are copied.
   - **Example:** `cp file1.txt /destination/folder`

2. **mv (Move)**
   - **Syntax:** `mv [options] source destination`
   - **Function:** Moves files or directories from one location to another.
   - **Options:**
     - `-i`: Prompts before overwriting existing files.
     - `-v`: Verbose mode, shows files as they are moved.
   - **Example:** `mv file1.txt /destination/folder`

3. **head**
   - **Function:** Outputs the first part of files.
   - **Syntax:** `head [options] [file(s)]`
   - **Options:**
     - `-n`: Specifies the number of lines to display.
   - **Example:** `head -n 10 file.txt`

4. **tail**
   - **Function:** Outputs the last part of files.
   - **Syntax:** `tail [options] [file(s)]`
   - **Options:**
     - `-n`: Specifies the number of lines to display.
   - **Example:** `tail -n 20 file.txt`

5. **sort**
   - **Function:** Sorts lines of text files.
   - **Syntax:** `sort [options] [file(s)]`
   - **Options:**
     - `-r`: Reverse the result of comparisons.
     - `-n`: Sort numerically.
   - **Example:** `sort -r file.txt`

6. **wc (Word Count)**
   - **Function:** Prints newline, word, and byte counts for each file.
   - **Syntax:** `wc [options] [file(s)]`
   - **Options:**
     - `-l`: Displays the count of lines.
     - `-w`: Displays the count of words.
   - **Example:** `wc -l file.txt`

7. **cat (Concatenate)**
   - **Function:** Concatenates files and prints on the standard output.
   - **Syntax:** `cat [options] [file(s)]`
   - **Options:**
     - `-n`: Number the output lines.
   - **Example:** `cat file1.txt file2.txt`

8. **tac**
   - **Function:** Concatenates and prints files in reverse.
   - **Syntax:** `tac [options] [file(s)]`
   - **Options:** None
   - **Example:** `tac file.txt`

9. **vi (Vim)**
   - **Function:** Text editor for Unix-like operating systems.
   - **Syntax:** `vi [file]`
   - **Usage:** Enters Vim text editor for specified file.
   - **Note:** Vim has different modes (command mode, insert mode, and more).

10. **nano**
    - **Function:** Simple text editor for Unix-like operating systems.
    - **Syntax:** `nano [file]`
    - **Usage:** Opens specified file in the nano text editor.
    - **Note:** Nano is more user-friendly for beginners compared to Vim.

11. **grep**
    - **Function:** Searches for patterns in files.
    - **Syntax:** `grep [options] pattern [file(s)]`
    - **Options:**
      - `-i`: Ignores case distinctions.
      - `-v`: Inverts the match.
    - **Example:** `grep -i "pattern" file.txt`

12. **vim**
    - **Function:** Improved version of the vi text editor.
    - **Syntax:** `vim [file]`
    - **Usage:** Opens specified file in the Vim text editor.
    - **Note:** Vim is highly customizable and has powerful features for advanced users.

13. **find**
    - **Function:** Searches for files and directories in a directory hierarchy.
    - **Syntax:** `find [path...] [expression]`
    - **Example:** `find /home/user -name "*.txt"` (Searches for all text files in the user's home directory)


# shell-snippets
Shell Snippets

## Source
https://youtu.be/Z56Jmr9Z34Q
https://youtu.be/kgII-YWo3Zw

## Example

### Standard
- date
- echo 'Hello World
- echo $PATH
- which echo
- --help
- sudo

### Navigation
- pwd (print working directory)
- cd (change directory)
- cd .. (one directory back)
- cd ./home (change directory in the current directory
- ls (Lists files in the directory)
- ls -l (List files with extra information)
- cd ~ (Goes to home directory)
- cd - (Goes to the previous directory)
- mv current-name-folder new-name-folder (Change name or file of folder)
- cp (copy)
- rm (remove)
- clear (control l - also works)

### Creation
- echo "Hello" > hello.txt (creates file with hello) in current directory
- echo "Hello Again." > hello.txt (appents the file with new content)
- cat hello.txt (prints content of a file)
- ls | >> hello.txt (pipe)
- open hello.txt (open a file)
- open ./ (open current folder)

### Scripting in Bash
``` Bash
  foo=bar
  echo $foo
  // Prints out: 'Bar'
  
  echo "Value is $foo"
  // Print out: "Value is bar"
  
    echo 'Value is $foo'
  // Print out: "Value is $foo"
```


## Extra Information

Absolute Paths vs Relative Paths

Spaces are reserved with Scripting is Bash

Single space don't take in account variables


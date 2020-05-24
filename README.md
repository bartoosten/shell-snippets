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
- convert image.png image.jpg
- man mv (Show manuel for the move command, close with cmd -q)

### Navigation
- pwd (print working directory)
- cd (change directory)
- cd .. (one directory back)
- cd ./home (change directory in the current directory
- ls (Lists files in the directory)
- ls -l (List files with extra information)
- ls *.sh (Only files with .sh extension)
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
- source mcd.sh (load a script into your shell
- touch exmaple
- touch example-1 example-2
- touch example-{3,4,5}

### Scripting in Bash

Working with values
``` Bash
  foo=bar
  echo $foo
  // Prints out: 'Bar'
  
  echo "Value is $foo"
  // Print out: "Value is bar"
  
  echo 'Value is $foo'
  // Print out: "Value is $foo"
```

Creating a shell script
``` Shell
  mcd () {
      mkdir -p "$1"
      cd "$1"
  }
```

$1 is the first variable of a shell script.

$0 is the name of the file script itself.

----

Example.sh script that check files for foobar

``` Shell
    echo "Starting program at $(date)"

    echo "Running program $0 with $# arguments with pid $$"

    for file in "$@"; do
        grep foobar "$file" > /dev/null 2> /dev/null
        if [[ "$?" -ne 0]]; then
            echo "File $file does not have foobar, adding one"
            echo "# foobar" >> "$file"
        fi
    done
```


## Extra Information

Absolute Paths vs Relative Paths

Spaces are reserved with Scripting is Bash

Single space don't take in account variables

PID means process id $$


## Yellow programming language

Yellow is a programming language coded with Python


## Installation

### Install for Mac:<br/>
`$ git clone https://github.com/ColdGrub1384/Yellow.git; Yellow/Build_for_Mac`
<br/>

### Install for Linux:<br/>
`$ git clone https://github.com/ColdGrub1384/Yellow.git; Yellow/Build_for_Linux`

### Why use Yellow

Yellow translates a yl script to Python, so you can code Python and Yellow in same script, such as Markdown and HTML.</br>
Yellow is very simple, you can use shortcuts such as ```$``` to auto import ```os``` and run a shell command, or ```log``` to write a string to log file for script, and get path with ```_LOG``` or print with colors: ```console.failed``` etc. <br/>

    // Comment

    /* Multiline
    comment*/

    ```python
    console {
        "Hello World from Yellow "+_version
    }
    \\n
    name = keyboard{
        "What's your name? "
    }

    log{
        "Question asked!"
    }

    Logclose{}

    from sys import platform
    if {platform == "linux" or platform == "linux2" or platform == "darwin"}
        ${"clear"}
    else:
        ${"cls"}

    if {name == "Adrian"}:
        console.okGreen {
            "We have the same name!"
        }
    else:
        if {name == "Windows"}:
            console.failed {
                "Fuck you"
            }
        
        else:
            console.okBlue {
                "My name is Adrian"
            }
 
    console{_LOG}

    LOGFILE = open{
         _LOG,"r"
    }

    console {
        "LOG:\n"+LOGFILE.read{}
    }
    
    \\n
    \\n
    ```

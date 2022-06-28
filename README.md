# BASH SCRIPTS

**Various bash scripts that I use on my linux system.**


### Disclaimer

This repository is intended for my personal use, **YOU DO NOT WANT TO USE IT** to install on your own system, but use it as an inspiration to make your own. I have tried to document it as best as possible for learning purpose.

---

## How to install the bash scripts.

* Clone the repository.

````
git clone git@github.com:UbioZur/bash-scripts.git
````

* You can simply copy the folders you want into your `$XDG_BIN_HOME` or `$HOME/.local/bin`.

* You can also use the install script `install.sh` which will create the sym-link for each of the scripts.

````
Usage:  install.sh [-h]
        install.sh [-v] [--dry-run] [--no-color] [-q] [-l] [--log-file /path/to/log [--log-append]] [--root-ok]
               [-a] [--no-utils] [-g]
        install.sh [-v] [--dry-run] [--no-color] [-q] [-l] [--log-file /path/to/log [--log-append]] [--root-ok] [-u]
               [-a] [--no-utils] [-g]

Install my bash scripts in the local bin folder

Available options:

    -h, --help          FLAG, Print this help and exit
    -v, --verbose       FLAG, Print script debug info
    --dry-run           FLAG, Display the commands the script will run. ( Will create/delete the folders needed to avoid failure)
    --root-ok           FLAG, Allow script to be run as root, usefull for container CI.

Log options:

    --no-color          FLAG, Remove style and colors from output.
    -q, --quiet         FLAG, Non error logs are not output to stderr.
    -l, --log-to-file   FLAG, Write the log to a file (Default: /var/log/install.sh.log).
    --log-file          PARAM, File to write the log to (Also set the --log-to-file flag).
    --log-append        FLAG, Append the log to the file (Also set the --log-to-file flag).

Install options:

    -u, --uninstall     FLAG, Uninstall the program.
    -a, --all           FLAG, Install eveything.
    --no-utils          FLAG, Do not install the utils scripts.
    -g, --gui-utils     FLAG, Install the gui utils.

````

---

## Scripts available

### GUI SCRIPTS

Various scripts used for my GUI environment.

* `screenlock` use i3lock to lock the screen using Dracula theme background color.

### UTILS

* `vault-crypt` Securely archive or install SSH and GPG configurations files.

---

## TODO - Future Updates

* Rofi scripts

## License

The repo is release under the `MIT No Attribution` license.

````
MIT No Attribution License

Copyright (c) 2022 UbioZur

Permission is hereby granted, free of charge, to any person obtaining a copy of this
software and associated documentation files (the "Software"), to deal in the Software
without restriction, including without limitation the rights to use, copy, modify,
merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
````

TLDR: A short, permissive software license. Basically, you can do whatever you want.

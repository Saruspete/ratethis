# ratethis

Find the rate of generic text
Useful for /proc/interrupts, df, ifconfig, quota...


This script parse program / files / stream to find and displays trends between 2 iterations

## Usage and examples

ratethis [options] [--] < command | file | - >

Simple mode 

``ratethis /proc/interrupts``

Display statistics at the end

``ratethis -S -- df -k``

5sec wait time, normalize values to 1sec

``ratethis -w 5 -N -- /proc/``

## Options 

    Options:
    -h, --help       Display this help
    -V, --version    Display version of the tool
 
    -S, --stats      Display statistics at the end of the run
    -C, --nocolor    Do not display colorful results
    -H, --noheader   Do not display header on top of iterations results
    -f, --filestats  File where to log statistics
    -w, --wait       Time in sec to sleep between 2 iterations
 
    -O, --onlymatch  Display only matching lines
    -c, --config     Use the specified internal configuration (see help)
    -s, --separator  Set the separator (default = s)
    -m, --match      Set the pattern to be matched against


## Screenshots

![/proc/meminfo output](https://raw.githubusercontent.com/Saruspete/ratethis/master/doc/screen_meminfo.png)


## Author

Adrien Mahieux <adrien.mahieux@gmail.com>

https://github.com/Saruspete/ratethis


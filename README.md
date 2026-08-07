# Bash `progress`

A bash script that shows a progress bar or a spinner while a command is running.

> [!WARNING]
> This is made for learning purposes, it is fun and funky, DO NOT USE IT IN REAL LIFE

## Usage

```bash
Take a command to run and show an animation while the command is runing.

  Usage: progress [OPTIONS] [FLAGS]

  Example:
    progress bar -d 4 -c sleep 5


 OPTIONS:
  help: Print this message and exit.
  bar: Show a progress bar, takes a duration in seconds. Best for commands where time is known.
  spinner: Show a spinner, does not take a duration, best for commands where time is unknown.


  FLAGS:
    -d, --duration: The duration of the animation, any number greater then 1, in seconds.
    -c: Command to run.
    -h, --help: Print this message and exit.



 Made by theacebutler, Aug 2026
```

## Installation

```bash
# clone the repo
git clone https://github.com/theacebutler/bash-pro-bar
cd bash-pro-bar
# make executable
chmod +x progress
# run
./progress spinner -c sleep 5
```

## Bugs

- see [BUGS.md](./BUGS.md)

- pr's welcome

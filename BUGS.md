# BUGS IN `./progress`

1. In a case where the user chains commands with a `&&`, like:
   `progress spinner -c sleep && echo 'do something' && sleep 4`, the spinner
   will exit after the _first_ command runs and will keep the process hanging for
   the second `sleep 4`

2. In the progress bar, in the command time is < duration, the bar will not fill
   up and will exit with an incomplete bar, basically we need to find a way to
   get the time left until the end of the command without relying on the user
   to input the correct duration.

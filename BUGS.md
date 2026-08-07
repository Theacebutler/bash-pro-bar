# BUGS IN `./progress`

1. In a case where the user chains commands with a `&&`, like:
   `progress spinner -c sleep && echo 'do something' && sleep 4`, the spinner
   will exit after the _first_ command runs and will keep the process hanging for
   the second `sleep 4`


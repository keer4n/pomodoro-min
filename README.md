## Minimalistic pomodoro

This is a bash script that works as a minimal standard pomodoro application for i3wm.
i.e. it counts 25 mins for work and 5 minutes for break in a continuous loop 
with minimal distraction. 

### Requirements:

- `dunst` notification daemon
  Install the daemon with: 
  ```sh
  $pacman -S dunst
  ```
  To prevent the stacking of notifications, the `hide_duplicate_count = yes` config
  should be enabled in `dunstrc`. An example config is included in the repo.
 
### Usage:

 ```sh
 $pomodoro
 ```
 
It also supports your own variable work/break time schedule. Just pass it as argument as:

```sh
$pomodoro 45 10
```

This creates a timer with 45 minutes worktime and 10 minutes breaktime.

Warning: This script times with the sleep function without considering other time
spent. 


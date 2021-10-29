# i3wm-shutdown-options
##This is feature is for all the i3 users who have been struggling to set up customised shortcuts for shutdown,login and reboot options\
The snippet of code can be found down.\

#bindsym $mod+x mode "exit: [l]ogout, [r]eboot, [s]hutdown"\
mode "exit: [l]ogout, [r]eboot, [s]hutdown" {\

  bindsym l exec i3-msg exit
  bindsym r exec systemctl reboot
  bindsym s exec systemctl poweroff
  bindsym Escape mode "default"
  bindsym Return mode "default"
}
bindsym $mod+x mode "exit: [l]ogout, [r]eboot, [s]hutdown"





This is code of snippet for setting up the shortcuts,update the above code using the config file of i3wm.\
The path for the config file of i3wm is \
/home/_your_host_name/.config/i3/config \
Using any text editor you can edit the config file. \
If you need to set up customised shortcuts \

bindsym $Your_custom_shortcut exec command_name \


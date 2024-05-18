# eww-hyprland-workspace
Simple template for eww widget that supports Hyprland workspaces with urgent EWMH.

These simple scripts are designed to added urgent EWMH support for a Eww
workspaces widget.  The scripts monitor Hyprland events and alters the css class
name of the workspaces widget.  The logic and class names are assigned in line
***17-18*** of the `eww.yuck` file.  The class names are `urgent`, `current`, `occupied`,
and `empty`.  The `urgent` class is assigned to until that that workspace has been
focused or destroyed.  The others classes are assigned based on the workspace's
state.  Included is a simple `eww.scss` file that can be used to style the widget
depending on the class name.

## IMPORTANT (Please read.)
These scripts/template have been updated to the recently released
***Hyprland Tag: v0.40.0-111-g2ead1fd2, commits: 4717***.  The main change that
effects these scripts is the location of the Hyprland sockets.  I left the old
commands in the scripts commented out for reference.  ***(See the scripts for more
information.)***

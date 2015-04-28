obbrowser
=========

A simple script for Openbox which recursively browses the filesystem through pipe menus (with icons)

### Set-up:

* To use this script with Openbox, insert the following
   line in your "menu.xml" file:

        <menu id="obbrowser" label="Disk" execute="obbrowser"/>

* If you're using it with "obmenu-generator", insert the following
   line in your "schema.pl" file:

        {pipe => ["obbrowser", "Disk", "drive-harddisk"]},
        
* Reconfigure openbox:

        openbox --reconfigure

* For low-level options, check the configuration file:

          ~/.config/obbrowser/config.pl

### Usage:
```
obbrowser [dir]
```



| -> /
| ---> [boot](##boot-stuff)
| ---> etc
| ---> [media](##media)
| ---> home
| ---> [proc](##proc)
| ---> [sys](##sys,run)
| ---> [run](##sys,run)
| ---> [var](##var)

## Boot stuff

info and debugging files in /boot dir => config, System.map

## etc

/etc/skel => Contains skeleton files used to populate newly created home directories.

/etc/systemd => Contains or points to configuration scripts for starting, stopping system services when using systemd.

## media

/media => for usbs usw. (or /run/media/username)

## proc

proc is pseudo-filesystem (everything is in memory)

most information in files is only obtained when they are viewed

important for system monitoring

Important pseudo-files, including /proc/interrupts, /proc/meminfo, /proc/mounts, and /proc/partitions, provide an up-to-the-moment glimpse of the system's hardware.

Others, like /proc/filesystems and the /proc/sys/ directory, provide system configuration information and interfaces.

## sys, run

similar to /proc

## var

often changing data files like log files etc
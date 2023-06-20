
**Standard naming convention:**
```
<name>_<version>-<revision_number>_<architecture>.deb
```

## Commands:

### Install
```bash
sudo dpkg -i foobar.deb
```

would be used for either installing or upgrading the foobar package.  

If the package is not currently installed, then it will be installed. If the package is newer than the one currently installed, then it will be upgraded.
  

### Remove

```bash
sudo dpkg -r package
```
  
is used to remove all of an installed package except for its configuration files.

```bash
 sudo dpkg -P package
```
  
is used to remove all of an installed package, including its configuration files.
Note that -P stands for purge.


```bash
# List all packages installed:
$ dpkg -l

# List files installed in the wget package:
$ dpkg -L wget

# Show information about an installed package:
$ dpkg -s wget

# Show information about a package file:
$ dpkg -I webfs_1.21+ds1-8_amd64.deb

# List files in a package file:
$ dpkg -c webfs_1.21+ds1-8_amd64.deb

# Show what package owns the /etc/init/networking.conf file:
$ dpkg -S /etc/init/networking.conf

# Verify the installed package's integrity:
$ dpkg -V package
```
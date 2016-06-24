# Linux

### System information

The “uname” command stands for (Unix Name), print detailed information about the machine name, Operating System and Kernel.

```bash
$ uname -a
```

### Package management
#### Update System Packages
The ‘update‘ command is used to resynchronize the package index files from the their sources specified in /etc/apt/sources.list file. The update command fetched the packages from their locations and update the packages to newer version.
```bash
$ sudo apt-get update
```

#### Upgrade System Packages
The ‘upgrade‘ command is used to upgrade all the currently installed software packages on the system. Under any circumstances currently installed packages are not removed or packages which are not already installed neither retrieved and installed to satisfy upgrade dependencies
```bash
sudo apt-get upgrade
```

```bash
$ sudo apt-get dist-upgrade
```



#### Install Packages
```bash
 $ apt-get install <packagename>
```
#### Remove Package
To un-install software packages without removing their configuration files (for later re-use the same configuration). Use the ‘remove‘ command as shown.
```bash
$ sudo apt-get remove
```

#### Remove Package including Configs
To remove software packages including their configuration files, use the ‘purge‘ sub command as shown below.
```bash
$ sudo apt-get purge <package-name>
```

#### List Packages
To list all the available packages, type the following command.
```bash
$ apt-cache pkgnames
```

#### Check Package Information
For example, if you would like to check information of package along with it short description say (version number, check sums, size, installed size, category etc). Use ‘show‘ sub command as shown below.
```bash
$ apt-cache show netcat
```

#### Check Dependencies for Specific Packages
Use the ‘showpkg‘ sub command to check the dependencies for particular software packages. whether those dependencies packages are installed or not. For example, use the ‘showpkg‘ command along with package-name.
```bash
 $ apt-cache showpkg vsftpd
```


### Shutdown


Shutdown the system and turn the power off immediately

``` bash
$ shutdown -h now

```

Shutdown the system after 10 minutes.

```bash
$ shutdown -h +10

```

Reboot the system using shutdown command.

```bash
shutdown -r now
```

# DFIR ORC Configuration

To configure DFIR ORC, you need:
* configuration files in XML format, located in the "config" directory
* items to embed (especially DFIR-Orc binaries in 32 and 64 bits), stored in the "tools" directory
* check "output" directory is __empty__ (no DFIR-Orc build)

The configurations given as example here use Sysinternals "Autoruns" tools. You have to download and put it in the "tools" directory.

The "tools" directory must therefore contain the following files:
* DFIR-Orc_x64.exe
* DFIR-Orc_x86.exe
* autorunsc.exe

Finally, to generate a configured DFIR-Orc executable, you have to run
the "Configure.cmd" script (on a Windows system).  
The generated binary is created in the "output" directory.

# Use

From our prefered Windows workstation

```
git clone this_repo
```

In a CMD windows :

For an x64 build (you need a x64 Windows of course):

```
> cd dfir-orc-config
> Configure.cmd
```

For an x86 build :

```
> Configure_x86.cmd
```

Wait seconds... check the output directory (cut and paste out of the
output directory)

You can test __DFIR-Orc.exe__ ;)


## Authors and contributors

Authors and contributors are the same as listed in the
[AUTHORS file of GitHub repository of the source code](https://github.com/dfir-orc/dfir-orc/blob/master/AUTHORS.txt).

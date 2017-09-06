# SomuSysAdmin

My memoirs for everythign I know about Linux and System Administration.

## Essential File Management Tools

### Understanding Linux File System Layout
**root (/)** - Contains all other directories.
**/boot** - Contains everything the system needs to start up
**/usr** - Contains program files
**/etc** - Contains configuration files
**/home** - Contains a user’s files
**/mnt** - Used to manually mount devices
**/media** - Devices like optical discs get auto-mounted on the media directory

Unlike other OSs, the linux files system is designed as such that multiple devices can be
mounted on the same file system hierarchy. Thus, it’s possible to mount devices remotely
as well!

### Finding Files
The **find** command is used to find a file within a folder and its subdirectories. When the
starting point of the search is the root directory (/) then find will search the entire file system.
While the utility is extremely thorough, this may cause delays due to remote devices on the
network mounted on the file system.
1 $ find / -name "passwd"

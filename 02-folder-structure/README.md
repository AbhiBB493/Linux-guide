# Understanding the Folder Structure

### Explanation of System Directories

### **Symbolic Links (Less Significant)**
| Directory | Description |
|-----------|-------------|
| `/sbin -> /usr/sbin` | System binaries for administrative commands (linked to `/usr/sbin`). ### helps in managing your system as an adminstrator |
| `/bin -> /usr/bin` | Essential user binaries (linked to `/usr/bin`).  ## this also have commands like sbin, but these are not administrative commands, thic commands can have access to normal user as well in simple word non administartive commands or actions|
| `/lib -> /usr/lib` | Shared libraries and kernel modules (linked to `/usr/lib`). ### libraries used by linux kernel to interact with hardware or perform any action |

### **Important System Directories**
| Directory | Description |
|-----------|-------------|
| `/boot` | Stores files needed for booting the system (not relevant in containers). |
| `/usr` | Contains most user-installed applications and libraries. |
| `/var` | Stores logs, caches, and temporary files that change frequently. |
| `/etc` | Stores system configuration files. ## like settings in the mobile phones, using which we can change anything the filesystem. |

### **User & Application-Specific Directories**
| Directory | Description |
|-----------|-------------|
| `/home` | Default location for user home directories. |
| `/opt` | Used for installing optional third-party software. |
| `/srv` | Holds data for services like web servers (rarely used in containers). ## data that can be configuration files etc |
| `/root` | Home directory for the root user. |

### **Temporary & Volatile Directories**
| Directory | Description |
|-----------|-------------|
| `/tmp` | Temporary files (cleared on reboot). |
| `/run` | Holds runtime data for processes. |
| `/proc` | Virtual filesystem for process and system information. |
| `/sys` | Virtual filesystem for hardware and kernel information. |
| `/dev` | Contains device files (e.g., `/dev/null`, `/dev/sda`). |

### **Mount Points**
| Directory | Description |
|-----------|-------------|
| `/mnt` | Temporary mount point for external filesystems.## to add more volumes(disks)|
| `/media` | Mount point for removable media (USB, CDs). ## adding audio files, mp4 etc |
| `/data` | Likely your **mounted volume** from Windows (`C:/ubuntu-data`). ## to store any data |

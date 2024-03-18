-r, --read-only
           Mount the filesystem read-only. A synonym is -o ro.

           Note that, depending on the filesystem type, state and
           kernel behavior, the system may still write to the device.
           For example, ext3 and ext4 will replay the journal if the
           filesystem is dirty. To prevent this kind of write access,
           you may want to mount an ext3 or ext4 filesystem with the
           ro,noload mount options or set the block device itself to
           read-only mode, see the blockdev(8) command.


-w, --rw, --read-write
           Mount the filesystem read/write. Read-write is the kernel
           default and the mount default is to try read-only if the
           previous mount(2) syscall with read-write flags on
           write-protected devices failed.

           A synonym is -o rw.

           Note that specifying -w on the command line forces mount to
           never try read-only mount on write-protected devices or
           already mounted read-only filesystems.


-t, --types fstype
           The argument following the -t is used to indicate the filesystem type. The filesystem types which are currently supported depend on the running kernel. See
           /proc/filesystems and /lib/modules/$(uname -r)/kernel/fs for a complete list of the filesystems. The most common are ext2, ext3, ext4, xfs, btrfs, vfat,
           sysfs, proc, nfs and cifs.

           The programs mount and umount(8) support filesystem subtypes. The subtype is defined by a '.subtype' suffix. For example 'fuse.sshfs'. It’s recommended to
           use subtype notation rather than add any prefix to the mount source (for example 'sshfs#example.com' is deprecated).

           If no -t option is given, or if the auto type is specified, mount will try to guess the desired type. mount uses the libblkid(3) library for guessing the
           filesystem type; if that does not turn up anything that looks familiar, mount will try to read the file /etc/filesystems, or, if that does not exist,
           /proc/filesystems. All of the filesystem types listed there will be tried, except for those that are labeled "nodev" (e.g. devpts, proc and nfs). If
           /etc/filesystems ends in a line with a single *, mount will read /proc/filesystems afterwards. While trying, all filesystem types will be mounted with the
           mount option silent.

           The auto type may be useful for user-mounted floppies. Creating a file /etc/filesystems can be useful to change the probe order (e.g., to try vfat before
           msdos or ext3 before ext2) or if you use a kernel module autoloader.

           More than one type may be specified in a comma-separated list, for the -t option as well as in an /etc/fstab entry. The list of filesystem types for the -t
           option can be prefixed with no to specify the filesystem types on which no action should be taken. The prefix no has no effect when specified in an
           /etc/fstab entry.

           The prefix no can be meaningful with the -a option. For example, the command

-B, --bind
           Remount a subtree somewhere else (so that its contents are
           available in both places). See above, under Bind mounts.

/dev/sdX - файл накопителя данных, X - это буква накопителя

/dev/sdXN - файл раздела накопителя данных, N - это номер раздела

Подмонтировать каталог к каталогу

mount --bind <исходный каталог> <каталог назначенияы>
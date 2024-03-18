fdisk - manipulate disk partition table

fdisk [options] device

fdisk -l [device...]


-l, --list
           List the partition tables for the specified devices and then exit.

           If no devices are given, the devices mentioned in /proc/partitions (if this file exists) are used. Devices are always listed in the order in
           which they are specified on the command-line, or by the kernel listed in /proc/partitions.


Command (m for help): m

Generic
   d   delete a partition
   n   add a new partition
   p   print the partition table
   t   change a partition type
   

Save & Exit
   w   write table to disk and exit
   q   quit without saving changes

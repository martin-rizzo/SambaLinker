# zzsamba

The "zzsamba" script is responsible for accessing disks on a Samba file server. It has three possible subcommands that must be specified as the first parameter.

## Usage

    zzsamba <subcommand> [<argument>]

The subcommands are:

- `list`: Lists the disks on the server that can be accessed by the user.
- `mount <disk>`: Mounts one of those disks.
- `umount <disk>`: Unmounts any of those disks.

## Examples

### Listing available disks

To list the available disks on the server, use the `list` subcommand:

    zzsamba list

This command will display a list of disks that the user can access.

### Mounting a disk

To mount a disk on the server, use the `mount` subcommand and provide the disk name as an argument:

    zzsamba mount disk1

This command will mount the disk named "disk1" to a local directory.

### Unmounting a disk

To unmount a disk on the server, use the `umount` subcommand and provide the disk name as an argument:

    zzsamba umount disk1

This command will unmount the disk named "disk1" that is mounted in the local directory.

## Requirements

This script requires the system to have the Samba client (`smbclient`) installed in order to access the disks on the server.

## Contributions

Feel free to contribute to this project. If you have any ideas or suggestions, open an issue or submit a pull request.

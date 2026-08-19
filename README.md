GPFS mmsdrestore service, for diskless nodes to restore GPFS confiurations and start mounting.

/etc/systemd/system/gpfs-diskless-restore.service

/etc/systemd/system/gpfs.service.d/gpfs-diskless.conf

and

gpfs-diskless-restore, save it to /usr/local/sbin, or elsewhere, but update the pfs-diskless-restore.service file.


In ./local-backup/ folder, they are for backup and restore to/from local CCR backup, with better performance.

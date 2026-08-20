# 1 

GPFS mmsdrestore service, from GPFS config/mgmt server, for diskless nodes to restore GPFS confiurations and start mounting.

/etc/systemd/system/gpfs-diskless-restore.service

/etc/systemd/system/gpfs.service.d/gpfs-diskless.conf

and

gpfs-diskless-restore, save it to /usr/local/sbin, or elsewhere, but update the pfs-diskless-restore.service file.

# 2

In ./local-backup/ folder, they are for backup and restore to/from local CCR backup, with better performance.

# 3

One caveat : 
 
You need to set the GPFS client cluster quorum node(s) can be SSH key accessed from all the client nodes.

If you can not set up like this, then look into the LOCAL version in the "local-backup" folder here.

For the "local-backup", if you use diskless PXE booting, then you need to find a way to sync the newest backup file into the image.
 

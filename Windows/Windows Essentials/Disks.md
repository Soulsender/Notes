#hardware
- RAID 0 (aka "striping") - files are split across disks so they are faster to access
	- fastest to access - no fault tolerance
- RAID 1 (aka "mirrored") - provides fault tolerance on between 2-32 disks by mirroring data onto two disks, cannot be shurk or extended, limited to 2 disks
	- provides fault tolerance
- RAID 5 (aka "striping with parity") - provides benefits of both RAID 0 and RAID 1, cannot be extended, mirrored, or shrunk
	- fast and provides fault tolerance
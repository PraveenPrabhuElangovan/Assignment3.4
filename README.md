1)Importance of namenode in Hadoop cluster:
NAMENODE is the master node It is responsible for proper functioning of cluster
a)	It processes the client requests
b)	It contains METADATA. It does this by containing Fsimage and edit logs editLogs It contains all transactions done on data It keeps a copy of itself in the hard disk FSImage It contains the screenshop of all block at the start before any start of transaction, and it sends a copy to secondary name node so that if primary name node fails this secondary name node could be used.
c)	So if primary name node fails there will be a loss. To avoid this in hadoop 2.x version there is a process known as high availability where there are 2 name node namely active and pasive name node(stand by) and the heart beat from data node are send to both these nodes 
d)	Name node also maintains the blocks(heart beat management and block replication ,reporting etc)

2)commands for HDFS:
	I attached screenshot for some of the basic commands

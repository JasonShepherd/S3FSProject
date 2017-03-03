This is instructions on how to run this application, these instructions assume you to have 
s3fs and fuse set up on your machine properly. 
WARNING This application is still in beta with some bugs so for now you can only encrypt a file 

to move a program to aws you need to do the following 

open up the terminal -> sudo s3fs bucketname /mnt/bucketname
to see if this is successful go to file sysytem/mnt your bucket folder should now be a binary file
To move a file up to amazon  create a document in your home folder
next open up the terminal and type the following:
sudo mv "document-name" /mnt/bucketname
next log into to your aws account and and go to management console 
select S3 click on your bucket name your file should be in there 
To see if it is encrypted download your file or just open it up on the 	amazon website


**note if you get a bad end point connection try the following
unmount bucket uding following command sudo fusermount -u /mnt/osfinal
Then remount the bucket again




# Hey! I'm Filing Here

In this lab, I successfully implemented the following TODO

## Building

In order to build, run make 
```
make
```

## Running

To create the image of the file system after running make
```
./ext2-create.img
```

In order to see the informaion held within the file system, run

```
dumpe2fs cs111-base.img
```

In order to check the file for any errors, run
```
fsck.ext2 cs111-base.img
```

To actually mount the file system, you can:
1) Make the directory
```
mkdir directory-name 
```
2) Mount the directory:
```
sudo mount -o loop cs111-base.img directory-name
```

## Cleaning up
In order to clean up the executable and object files:
```
make clean
```

To unmount the file system if you craeted it:

```
sudo umount directory-name
rmdir directory-name
```

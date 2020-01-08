# fat32images
FAT32 images

This repo contains various blank disk images, each containing a single FAT32 partition of a different size as depicted by the image name.
These images can be written to an SD card using Balena Etcher, Win32diskimager, or even dd if using Linux.
By doing so, the FAT32 partition is created on the SD card.

This is particularly useful for creating FAT32 partitions on SD cards >32GB in size, which are typically formatted as exFAT when 
formatted as a whole, due to their size.

Once formatted in this way, such large SD cards are suitable for copying NOOBS files to for the Raspberry Pi.

The `createfat32` file is a linux bash script that is used to create the images. It is passed a single parameter which specifies the size of the image to be created in GBs.

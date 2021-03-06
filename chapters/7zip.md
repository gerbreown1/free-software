# How to manage your files with FREE archive and compression software.

## Is your hard drive becoming full?

### Below are listed 3 things you can do to get more space.

1. **Buy a new hard drive.**
Even though prices of hard drive are coming down, it would still be and additional expense.  If you were to choose an internal drive it would require expertise in installing hardware in your computer and then you would have the problem of transferring the files from the old drive to the new one.

1. **Delete old or unnecessary files.**  
This is something we all should do on a regular basis. A lot of applications create temporary files with the ".tmp" extension.  These can be safely deleted. Web browsers create "cache" files that can also be deleted.

1. **Use an archive and compression program.**  
This is the method I am recommending in this article.

## Are your e-mail attachments too large to send with a regular e-mail?  
See number 3 above for a solution to this problem.

## The application this article is about is the archive and compression application called 7-Zip.

### What can it do for you?
This will create compressed archives of the files you select. The original files can then be deleted or moved to another source thereby saving disk space for you. The compressed and archived file can also be copied to another place such as to the cloud.

### What Operating System is it for? 
Linux (Numerous distros), Mac OS X and Windows (Numerous versions)

### Where can you to get it?

[http://www.7-zip.org/download.html](http://www.7-zip.org/download.html)
At this page you can select the correct version for your operating system.

## The main features of 7-Zip

* High compression ratio in 7z format with LZMA and LZMA2 compression
* Supported formats:
    * Packing / unpacking: 7z, XZ, BZIP2, GZIP, TAR, ZIP and WIM
    * Unpacking only: ARJ, CAB, CHM, CPIO, CramFS, DEB, DMG, FAT, HFS, ISO, LZH, LZMA, MBR, MSI, NSIS, NTFS, RAR, RPM, SquashFS, UDF, VHD, WIM, XAR and Z.
* For ZIP and GZIP formats, 7-Zip provides a compression ratio which is 2-10 % better than the ratio provided by PKZip and WinZip
* Strong AES-256 encryption in 7z and ZIP formats
* Self-extracting capability for 7z format
* Integration with Windows Shell
* Powerful File Manager
* Powerful command line version
* Plugin for FAR Manager
* Localizations for 79 languages

## Compression table

On the web site is a table showing the compression ratios of various compressing programs.  

For the same set of 161 files @ 15,684,168 bytes the compressed size is 4,621,135 for a ratio of 100%. 

The next competitor, WinRAR created a compressed size of 5,021,556 bytes. WinZip (maximum-portable) created a file of 6,448,666 bytes.

Quote from the 7-zip.org website: "Compression ratio results are very dependent upon the data used for the tests. Usually, 7-Zip compresses to 7z format 30-70% better than to zip format. And 7-Zip compresses to zip format 2-10% better than most of other zip compatible programs."

## Versions for other operating systems.

For use with Ubuntu or other Debian versions of Linux it is recommended to use the system's Snyaptic Package Manager to download and install 7zip-full on your system instead of installing it manually from the web site as there are a lot of dependent files required.

There is a website that has RPM packages of Fedora, however it was last updated 2011.01.06 so it is quite obsolete. As I don't use Fedora, I'm not aware if it is available in the repository as a RPM package.

There are also 2 websites for Mac OS X listed.  The first one says he is no longer maintaining the Mac version of 7Zip and the other one was last updated in March 2008.

Even on the sourceforge.net website the latest version is listed as 9.20.1 and it is also dated 2011-03-16.

### p7zip on my Ubuntu system

I just did a check on trying to install it on my Ubuntu 14.04 system and received the message stating p7zip is already the newest version.

I have not used p7zip for awhile but when I did I thought it did a very good job of compressing files when using the 7z format as opposed to using the zip format.

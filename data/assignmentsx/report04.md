#Disk Encryption for Linux
by Gurjap

##Explain/define the topic?    
In 2012 IBM (International Business Machines) made all the employees that were provided a laptop to implement Full-Disk encryption for their primary hard drive, and any other drive, internal or external that had sensitive information. The original laptops ran a dual boot that contained windows and Linux, however, the dual boot environment won’t work for Full-Disk Encryption. For those who require both operating systems, they would have to choose one as the primary operating system and then run the other as a guest virtual machine. 

##Who is behind it? corp, product, individual
The corporation of IBM is behind the disk encryption for the employees. The international business machine is a corporation that manufactures and markets computers hardware, middleware and software, and offers hosting and consulting services in areas ranging from mainframe computer to nanotechnology.  The corporation of IBM wanted to protect the data on the primary hard drive, and any other drive, internal or external that has sensitive information just in case they got hacked or lost the laptops. There was an exception for employees who did not take their laptops outside of the buildings because they were always secure. 

##What do they hope to achieve? 
IBM hopes to achieve more security for their employees and the sensitive data involved at IBM. IBM has around 434 thousand employees working, so achieving disk encryption is important or else a lot of data can be lost or manipulated for mischievous reasons to hurt the corporation. With the disk encryption at IBM, they also hope to achieve a reputable status with keeping the information secure. This will help build more trust with the employees and clients that relate to IBM and can relate to more work. A client would not want to trust a corporation that does not have encrypted data for security, so IBM would like to give that sense of relief to its clients. 

##Where do they/it stand?
After all, this took place there were a lot of pros and cons to the disk encryption. The cons were, that the implementation is a full re-install of Linux, followed by a fresh install of windows. Along with the learning curve, that was required to learn Linux as its different from Windows. Lastly, not all jobs at IBM ran on Linux, so windows OS was still needed and running windows on a VM guest with limited memory resources was extremely slow compared to running it on a fully-encrypted disk. With all these cons also came a lot of pros. The pros of this switch were that LUKS or Linux unified key setup (disk encryption) allowed up to 8 passphrases, which you can give to different people in the company. Linux is also a solid operating system and is more secure against viruses. Furthermore, employees that work with multiple clients can have separate windows guest for each one, preventing cross-contamination between systems. 

##How to use or play with the tech? 
Implementing LUKS encryption on your Linux laptop is not that bad. The first step in implementing LUKS encryption on your Linux laptop is to back up your system. Backup all the files, including programs, bookmarks, and operating settings to an external disk drive. After the backup is completed you will need to Re-Partition the drive. You can do this in two parts, the first part being a small unencrypted partition of 2gb that will hold the Master Boot Record, Grand Unified Bootloader, and the /boot directory.  The second part will be the rest of the drive which is also referred to as a physical volume.  Later, you will create logical volumes in the LVM container. You can create three logical volumes on the encrypted physical container: swap, slash (/) directory and home (/home). This step will be followed by a Linux installation and a windows guest KVM image. To do the windows guest KVM image you can open client for Linux and select on the Windows operating system and click install. After clicking install you will get a fresh install of windows operating system on a 30gb raw image file. You will need to set up file sharing between Linux and windows and transfer all your files back. You can use the original eternal drive from the start to bring your data back to the home directory. Lastly, you will need to protect your encryption setup. You will need to add a second passphrase; the first passphrase will be a long passphrase that you remember, and the second passphrase will be an even longer one that will be given to your boss or admin assistant in case something happens to you. You should also backup the crypto header which is a small section in front that contains your passphrases, so if its corrupted you would not be able to access the rest of your data. You should create a backup image file and store it on an encrypted USB memory stick or external drive. Further reading? unordered list, 3-6 links

##Further Reading? Unordered list, 3-6 links
- https://www.ibm.com/storage/data-encryption
- https://knowledgelayer.softlayer.com/procedure/use-luks-red-hat-enterprise-linux-6-full-disk-encryption
- https://books.google.ca/books?id=bFjAAgAAQBAJ&pg=PA273&lpg=PA273&dq=ibm+disk+encryption+for+linux&source=bl&ots=3ow0W8caSJ&sig=_ITUX_sNf4Jf30tfUaE_5h0ZQ4A&hl=en&sa=X&ved=0ahUKEwiiy4aa9JTXAhUN2GMKHXFRDUEQ6AEIZDAJ#v=onepage&q=ibm%20disk%20encryption%20for%20linux&f=false
- https://www.pcworld.com/article/3140023/linux/3-encryption-tools-for-linux-that-will-keep-your-data-safe.html

<img src="/pix/reports/04-1.png" />
# carp

A simple guide to transferring files from a Mac to a Windows PC using a USB drive.

## What you need

- A USB flash drive with enough free space for your files.
- Access to both the Mac and the Windows PC.

## Prepare the USB drive

If the drive is new or can be erased, format it as **exFAT** so both macOS and Windows can read and write it. Formatting erases everything on the drive, so copy off any files you need first.

### On a Mac

1. Connect the USB drive.
2. Open **Disk Utility** (Applications → Utilities).
3. Choose **View → Show All Devices** if needed, then select the USB drive.
4. Click **Erase**. Choose **exFAT** as the format and **Master Boot Record (MBR)** as the scheme for broad compatibility.
5. Confirm **Erase**. Double-check that you selected the USB drive, not your Mac's internal disk.

If the drive already uses exFAT, you can skip formatting.

## Copy files from the Mac

1. Open **Finder** and locate the files or folders you want to transfer.
2. Drag them onto the USB drive in Finder, or copy and paste them.
3. Wait for the copy to finish.
4. In Finder, click the eject icon next to the USB drive and wait until it disappears before unplugging it.

## Copy files to the Windows PC

1. Plug the USB drive into the Windows PC.
2. Open **File Explorer** and select the USB drive under **This PC**.
3. Copy the files to a folder on the PC, such as **Documents** or **Pictures**.
4. When copying is complete, use **Safely Remove Hardware and Eject Media** in the Windows taskbar before unplugging the drive.

## Troubleshooting

- **The drive does not appear on Windows:** Try another USB port. If the drive is formatted as APFS or Mac OS Extended, Windows may not read it; use exFAT after backing up its contents.
- **A file will not copy:** Check that the USB drive has enough free space and that the file is not larger than 4 GB if the drive is formatted as FAT32. exFAT supports larger files.
- **The drive asks to be formatted:** Do not format it if it contains files you need. Formatting erases the drive; connect it to the Mac and copy the files elsewhere first.

Always eject the drive before unplugging it to reduce the chance of file corruption.

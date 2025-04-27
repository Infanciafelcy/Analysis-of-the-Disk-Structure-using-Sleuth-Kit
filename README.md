# Analysis-of-the-Disk-Structure-using-Sleuth-Kit
# Name: Infancia felcy P
# Reg no: 212223040067
## AIM:
To analyze the disk structure of a given disk image using Sleuth Kit tools in Kali Linux.

## DESIGN STEPS:
### Step 1:
Obtain or create a disk image file (e.g., disk.dd) to analyze. Open the terminal in Kali Linux.

### Step 2:
Use Sleuth Kit tools like mmls, fsstat, and fls to examine the partition layout, file system details, and file listing.

### Step 3:
Interpret the output of the tools to understand the disk structure, including partitions, sectors, and files.

## PROGRAM:
Sleuth Kit Disk Analysis Commands
leuth Kit Disk Analysis Commands

✅ Option 1: Create a Sample Disk Image (for Testing)

Let’s create a 10MB blank disk image and simulate file system activity:

cd ~/Downloads

# Step 1: Create an empty disk image
dd if=/dev/zero of=disk.dd bs=1M count=10

# Step 2: Format it with a file system (like FAT32)
mkfs.vfat disk.dd

## OUTPUT:
Disk Structure Analysis Results
![image](https://github.com/user-attachments/assets/5d9f9e04-dfa1-417f-8b73-898c9acc0cbc)
![image](https://github.com/user-attachments/assets/6e407f69-cca3-4367-9e7c-9f2bc9ad6e6f)
# mmls
```
mmls disk.dd
```
# fls
```
fls -f fat -o 0 disk.dd
```
![image](https://github.com/user-attachments/assets/147cbd4c-0c5e-4403-9c99-897bf7bff15a)
![image](https://github.com/user-attachments/assets/18c55746-6dbc-45be-af35-279ce9fab397)
![image](https://github.com/user-attachments/assets/5124daa2-e269-45dc-aa74-2c39f65285c0)
![image](https://github.com/user-attachments/assets/9a4c01f9-bde1-472b-a19d-f2313d9e8169)
![image](https://github.com/user-attachments/assets/958f360a-3694-41d0-86ba-285236a417f1)


## RESULT:
The analysis was performed successfully using Sleuth Kit, and the disk structure was understood in detail.

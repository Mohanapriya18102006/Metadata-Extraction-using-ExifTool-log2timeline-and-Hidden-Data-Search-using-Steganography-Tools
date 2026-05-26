# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
## AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.
## REQUIREMENTS

- Operating System: Windows 10/11, macOS, or Linux

- Tool: Autopsy Digital Forensics
- Test Data: Disk image file ( disk.dd , disk.img , .E01 )
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Install Autopsy]
    B --> C[Create New Case in Autopsy]
    C --> D[Add Data Source: Disk Image]
    D --> E["Run File System & Data Recovery Modules"]
    E --> F[Locate Deleted Files in Results]
    F --> G[Recover and Export Deleted Files]
```

## DESIGN STEPS:
### Step 1:
Open Autopsy and create a new case with appropriate case details.

### Step 2:
Add a disk image as a data source and let Autopsy analyze the content.

### Step 3:
Navigate to the "Deleted Files" section in Autopsy and examine or recover the deleted files.

## PROGRAM:
### Install Autopsy
```bash
# Download Autopsy from:
# https://www.autopsy.com/
# Install following the setup wizard.
```
### Create a New Case
```
# File → New Case
# Enter Case Name: Deleted_File_Recovery
# Choose Base Directory: C:\Cases\Deleted_File_Recovery
# Click Finish
```
### Add Disk Image
```
# Add Data Source → Disk Image or VM File
# Browse to: C:\forensics\disk.dd
# Click Next
```
### Run Ingest Modules
```# Select:
# - File System Analysis
# - Keyword Search (optional)
# - Data Recovery / Carving
# Click Finish
```

## Output:

Install and launch autopsy

<img width="1920" height="1200" alt="Screenshot (40)" src="https://github.com/user-attachments/assets/3c1f36ee-891a-446a-ad0f-66804ad0146c" />

Create case information

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/0bf081f5-c5b7-4f60-afdb-91412f2c7f44" />

Select data source type

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/54e2cb90-22db-4ed8-930f-66167e29f3e0" />

Add data souce

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/f42a133b-b168-4ed4-851a-2c58f9e897d3" />

Metadata Extraction

<img width="1920" height="1200" alt="Screenshot (59)" src="https://github.com/user-attachments/assets/61511026-a0d3-400f-af72-314e806b17a4" />

Timeline analysis

<img width="1920" height="1200" alt="Screenshot (57)" src="https://github.com/user-attachments/assets/ff226169-6ec3-4725-bdae-40da33c966f0" />

Keyword Search

<img width="1920" height="1200" alt="Screenshot (60)" src="https://github.com/user-attachments/assets/4e443f50-62fa-441e-b122-a7d59c17acd8" />
<img width="1920" height="1200" alt="Screenshot (61)" src="https://github.com/user-attachments/assets/e6168bad-a002-470c-96ad-a75d6c0f4404" />



## RESULT:


Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using autopsy

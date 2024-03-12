The File Archiver is a Python script that recursively iterates through a directory tree, collects all text files, and archives them into a ZIP file. It utilizes the pathlib module for file path manipulation and the zipfile module for creating and managing ZIP archives.

Clone the repo:

``git clone https://github.com/your-username/file-archiver.git``

Run the script:

``python file_archiver.py``

Features:

- Recursively iterates through a directory and its subdirectories to collect text files.
- Creates a ZIP archive containing all collected text files.
- Deletes the original text files after archiving them to save disk space.

Config:

- Modify the root_dir variable to specify the directory containing the text files to be archived.
- Adjust the file extension pattern in the rglob() function to match the desired file type(s) for archiving.

Ex., Suppose you have the following directory structure:

``files/
    ├── folder1/
    │   ├── file1.txt
    │   └── file2.txt
    ├── folder2/
    │   ├── file3.txt
    │   └── file4.txt
    └── file5.txt
``

After running the script, the text files will be archived into a ZIP file named archive.zip, and the original text files will be deleted:

``files/
    ├── archive.zip
``

**#MyFS - A Custom Filesystem Implementation**
**Overview**
Welcome to MyFS, a custom filesystem implementation project developed in C++. This project simulates a simple filesystem in userspace, providing basic file management capabilities such as creating, editing, listing, and deleting files and directories. The project is designed to mimic some core features of a traditional filesystem, offering a practical learning experience in understanding how filesystems work at a fundamental level.

**Features**
File and Directory Management: Create, list, edit, and delete files and directories.
Simulated Block Device: Uses a file to simulate a block device, providing a realistic environment for testing filesystem operations.
Simple Command Interface: Interact with the filesystem through a straightforward command-line interface.
Persistence: Ensure that file data and metadata persist between sessions.
Key Components
myfs.h & myfs.cpp: Core implementation of the MyFS filesystem, including methods for file and directory operations.
vfs.h & vfs.cpp: Virtual filesystem interface handling user commands and interfacing with the MyFS implementation.
blkdev.h & blkdev.cpp: Simulation of a block device, representing the storage medium for the filesystem.
Getting Started
To get started with MyFS, follow these steps:

Clone the Repository:

sh
Copy code
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
Build the Project:

sh
Copy code
mkdir build
cd build
cmake ..
make
Run the Filesystem Simulator:

sh
Copy code
./bin/myfs /tmp/myfs_data
This command starts the MyFS simulator, storing data in the specified file (/tmp/myfs_data).
**
Use the Command Interface:**

touch <filename>: Create a new file.
edit <filename>: Edit the contents of a file.
cat <filename>: Display the contents of a file.
ls [<directory>]: List the contents of a directory.
rm <filename>: Remove a file.
mkdir <directory>: Create a new directory.
rmdir <directory>: Remove a directory and its contents.
mv <source> <destination>: Move or rename a file or directory.
Learning Objectives
This project was developed as an educational exercise to understand the principles of filesystem design, including:

Filesystem Structure: Understanding how filesystems organize and manage data.
Block Device Simulation: Learning how filesystems interact with storage media.
File Operations: Implementing basic file operations such as creation, deletion, and modification.
Data Persistence: Ensuring data consistency and persistence across sessions.
Contributions and Feedback
Contributions are welcome! If you have suggestions, improvements, or encounter issues, please feel free to open an issue or submit a pull request. Your feedback is valuable and helps improve this project.

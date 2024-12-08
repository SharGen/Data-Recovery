This data recovery tool is designed to search for specific file types (e.g., PDF, JPG, ZIP, PNG) on a removable drive by identifying their unique file signatures and recovering the data to a designated location. The program begins by identifying all available drives on the system and prompts the user to specify the letter of the removable drive they want to scan. Upon receiving input, it simulates a loading process via a progress bar before launching multiple threads to scan and recover data efficiently.

The recovery process is handled by the `DataRecovery` method, which reads the specified drive byte by byte in chunks of 512 bytes. It searches for the signature of a target file type by looking for its unique starting and ending bytes (commonly referred to as magic numbers). When the program detects the start of a file, it begins extracting the content, continuing until it finds the end signature of the file. The recovered file is written to a new location on the host system, avoiding overwriting existing data. This ensures precise recovery of files based on their boundaries.

To optimize performance, the program uses multithreading. Each thread is dedicated to recovering one type of file format simultaneously (e.g., one thread for PDFs, another for JPGs). This parallel approach reduces the time required to scan and recover multiple file types on a drive. Additionally, it ensures that the tool can handle various file formats without sequential processing bottlenecks. Once all threads complete their tasks, the program calculates the total time taken for the recovery operation, providing the user with a performance summary.

The tool also incorporates user-friendly elements such as a visual ASCII banner (using the `pyfiglet` library), clear progress bar updates, and detailed messages to indicate file discovery and recovery status. The recovered files are stored in a directory called `RecoveredData`, which is created in the current working directory if it does not already exist. This design makes the tool accessible to users, as they are guided through the process with clear instructions and visual feedback, ensuring ease of use even for non-technical individuals.

# To use source code

**Step 1**
Install pyfiglet*
>```pip install pyfiglet```

**Step 2**
Make sure to launch finshed code via admin terminal.

<img width="500" alt="image" src="https://user-images.githubusercontent.com/74583970/216753507-8ba39b5e-e94f-4842-823c-64a67626b92f.png">

As this line of code makes directory to the CWD or current working directory. It coud need admin perm if running it on root or restricted volume or directory.

# Please contribute and share :)

https://github.com/SharGen/Data-Recovery

https://www.linkedin.com/in/saransh-sinha-6b47b921b/

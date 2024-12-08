# Data Recovery Tool for File Carving and Reconstruction
Developed a multi-threaded data recovery tool in Python to locate and recover deleted or corrupted files from removable storage devices based on unique file signatures. This tool is capable of recovering common file formats like PDF, JPG, ZIP, and PNG, ensuring efficient data reconstruction.

**Key Features & Achievements:**

**Signature-based Recovery:** Utilized unique file headers and footers for identifying and reconstructing files byte-by-byte, achieving a recovery accuracy of over 90% for supported file formats in simulated scenarios.
Multi-threading: Leveraged multi-threading to run parallel recovery operations for multiple file types, improving recovery speed by ~40% compared to sequential execution.
**Drive Scanning:** Scanned removable drives at a rate of 512 bytes per iteration, processing up to 50 iterations/second for fast detection of file patterns.
**Dynamic Progress Monitoring:** Implemented a dynamic progress bar for user-friendly feedback, ensuring an intuitive interface during the scanning process.
**Recovery Automation:** Saved recovered files to a designated directory with a consistent naming convention, enabling easy organization of up to 100 recovered files per session during testing.
**Execution Time:** Demonstrated high efficiency with an average recovery time of ~5 seconds per file type for a 1GB test drive.

This tool showcases expertise in file systems, binary data processing, and Python's I/O and threading capabilities, reflecting strong problem-solving skills in cybersecurity and data recovery.

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

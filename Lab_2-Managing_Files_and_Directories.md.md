### Task 1: Create Directories
1. Open your terminal and ssh to **server1** as user **student**.
2. Create a directory in */home/student/* named `workspace`:
   ```bash
   mkdir -v ~/workspace
   ```
3. Inside `workspace`, create three subdirectories: `reports`, `logs`, and `configs`:
   ```bash
   cd workspace
   mkdir -v reports logs configs
   ```

### Task 2: Create Text Files
4. Navigate to the `reports` directory:
   ```bash
   cd reports
   ```
5. Create five text files named `report1.txt`, `report2.txt`, `report3.txt`, `summary.txt`, and `overview.txt`:
   ```bash
   touch report1.txt report2.txt report3.txt summary.txt overview.txt
   ```

6. Navigate to the `logs` directory:
   ```bash
   cd ../logs
   ```
7. Create five text files named `log1.txt`, `log2.txt`, `log3.txt`, `log4.txt`, and `log5.txt`:
   ```bash
   touch log1.txt log2.txt log3.txt log4.txt log5.txt
   ```

8. Navigate to the `configs` directory:
   ```bash
   cd ../configs
   ```
9. Create two text files named `config1.txt` and `config2.txt`:
   ```bash
   touch config1.txt config2.txt
   ```
10. Return to your home directory and confirm all the lab files and directories are created correctly:
    ```bash
    cd ~
    tree ~/workspace
    ```
### Task 3: Add Content to Files
11. Open `report1.txt` in a text editor (e.g., `nano` or `vim`) and add some sample content:
    ```plaintext
    Report 1: Things I Learned About Linux This Week.
    ```
12. Add content to `log1.txt` describing a log entry:
    ```plaintext
    Log Entry: Class started at 09:00 AM CT.
    ```

### Task 4: Move Files
13. Move `summary.txt` to the `configs` directory using relative paths:
    ```bash
    mv -v workspace/reports/summary.txt workspace/configs/
    ```

### Task 5: Copy Files
14. Copy `overview.txt` to the `logs` directory using absolute paths:
    ```bash
    cp -v /home/student/workspace/reports/overview.txt /home/student/workspace/logs/
    ```

### Task 6: Rename Files
15. Rename `config1.txt` to `settings.txt` while working in the *~/workspace/configs/* directory:
    ```bash
    cd ~/workspace/configs
    mv -v config1.txt settings.txt
    ```

### Task 7: List Files and Directories
16. List all files in the `reports` directory:
    ```bash
    ls ../reports
    ```
17. List all files in the `logs` directory:
    ```bash
    ls ../logs
    ```

### Task 8: Remove Files and Directories
18. Delete the `settings.txt` file:
    ```bash
    rm -v settings.txt
    ```
19. Remove the `logs` directory and its contents:
    ```bash
    rm -rv ../logs
    ```

### Task 9: Check Disk Usage
20. Check the disk usage of the `workspace` directory:
    ```bash
    du -sh ~/workspace
    ```

### Task 10: Find Files
21. Find all `.txt` files in the `workspace` directory:
    ```bash
    find ~/workspace -name "*.txt"
    ```

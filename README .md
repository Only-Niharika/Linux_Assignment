# Linux Assignment

This README documents Linux command-line exercises for navigation, file handling, permissions, search, system info, archiving, and networking.

## Task 1: Navigation and Directories

### Check current directory
```bash
pwd
```
Example output:
```text
/home/ubuntu
```

### List root directory
```bash
cd ..
cd ..
ls
```

### Go to home directory
```bash
cd /home
```

### Create `devops_practice` folder
```bash
cd Desktop
mkdir devops_practice
```

### Create 3 files inside `devops_practice`
```bash
cd devops_practice
touch demo.txt
touch info.txt
touch Niharika.txt
```

## Task 2: File Operations

### Create `logs` folder
```bash
mkdir logs
```

### Move `file1.txt` into `logs`
```bash
touch file1.txt
mv file1.txt logs/
```

### Rename `file2.txt` to `config.txt`
```bash
touch file2.txt
mv file2.txt config.txt
```

### Copy `file3.txt` to `backup.txt`
```bash
touch file3.txt
nano file3.txt
cp file3.txt backup.txt
```

### Delete `logs` folder
```bash
rm -r logs
```

## Task 3: File Content

### Write sample text in `config.txt`
```bash
nano config.txt
```

### Display content
```bash
cat config.txt
```

### Show first and last line
```bash
head -n 1 config.txt
tail -n 1 config.txt
```

## Task 4: Permissions

### Check permissions of `config.txt`
```bash
ls -l config.txt
```

### Allow only owner read and write
```bash
chmod 600 config.txt
```

## Task 5: Search and Find

### Search word `DevOps`
```bash
grep -r -i devops .
```

### Locate `config.txt` in system
```bash
sudo find /home -name config.txt
```

## Task 6: System Information

### Check username
```bash
whoami
```

### Check hostname
```bash
hostname
```

### List running processes
```bash
ps
```

### Check disk usage
```bash
df -h
```

### Check memory usage
```bash
free
```

## Task 7: Archive and Compress

### Create tar archive of `devops_practice`
```bash
tar -cvf devops_practice.tar devops_practice
```

### Compress and extract archive
```bash
gzip devops_practice.tar
tar -xvzf devops_practice.tar.gz
```

## Task 8: Networking

### Find IP address
```bash
ifconfig
```

### Ping Google (5 packets)
```bash
ping -c 5 google.com
```

### Check DNS resolution
```bash
dig google.com
```

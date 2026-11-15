# Mission 3 — Understand the Operating System

## 1. Task / Objective

The objective of this mission is to explore macOS, understand how an operating system manages processes, memory, storage, devices and permissions, and learn how files and folders are organized.

## 2. Work Completed

### Task 3.1 — Explore Your Operating System

- Identified the operating system as macOS.
- Recorded the operating system version and build information.
- Identified the active user account.
- Checked the available storage space.
- Observed running applications and system activity using Activity Monitor.

**System information:**
- Operating System: macOS
- Version: 27.2.1
- Build Version: 26B131
- Username: [Redacted]
- Available Storage: [Enter the value observed]

### Task 3.2 — Understand Processes

- Used Terminal commands to view running processes.
- Identified the PID (Process Identifier) column.
- Observed application processes such as Google Chrome and Slack.

**My Understanding:**

A process is a program that is currently being executed. A PID is a unique Process Identifier assigned to each process. Examples of processes include Google Chrome and Slack.

### Task 3.3 — Understand Paths and Permissions

- Used `pwd` to identify the current working directory.
- Used `cd` and `cd ..` to navigate between folders.
- Understood the difference between absolute and relative paths.
- Used `ls -l diary.txt` to inspect file permissions.

**My Understanding:**

An absolute path is the complete path starting from the root directory, whereas a relative path specifies a location in relation to the current working directory.

Observed permission string:

`-rw-r--r--`

- Owner (`rw-`): Read and write.
- Group (`r--`): Read only.
- Others (`r--`): Read only.

Permission symbols:
- `r` — Read
- `w` — Write
- `x` — Execute
- `-` — Permission not granted

### Task 3.4 — Explain OS Responsibilities

| Responsibility | Explanation | Example |
|---|---|---|
| Process Management | Manages running processes and distributes CPU time. | Running Chrome and Slack simultaneously. |
| Memory Management | Allocates and manages RAM for applications. | Allocating RAM to Chrome. |
| Device Management | Manages communication between hardware and the computer using device drivers. | Managing keyboard and mouse input. |
| File Management | Organizes, stores and retrieves files and folders. | Creating and saving files. |
| User Interface / Shell | Provides an interface for users to interact with the computer through GUI or CLI. | Finder and Terminal. |
| Security and Permissions | Controls access to system resources and files. | Read, write and execute permissions. |

## 3. Commands / Tools Used

- `pwd` — Displays the current working directory.
- `cd` — Changes the current directory.
- `cd ..` — Moves to the parent directory.
- `ls` — Lists files and folders.
- `ls -l` — Displays detailed file information and permissions.
- `ps` — Displays process information.
- Activity Monitor — Observes running applications and system activity.

## 4. My Understanding

An operating system manages the computer's hardware and software resources. It manages processes, memory, devices, files, user interaction and security. It allows different applications to run and helps the computer operate efficiently.

## 5. Difficulties Faced

- Understanding the difference between absolute and relative paths.
- Identifying familiar application processes among many running processes.
- Understanding the permission symbols in a detailed file listing.

## 6. How I Resolved Them

- Practised navigating between folders using `cd` and `cd ..`.
- Used process-filtering commands to identify Chrome and Slack.
- Studied the permission string using the `ls -l` command.

## 7. Evidence / Files

- Terminal outputs and relevant screenshots are saved in the project evidence folder.
- Screenshots should not expose personal usernames or other private information.

## 8. Commit Details

Commit Message: Document operating system and file management.


# Mission 2 — Become Comfortable with the Terminal

## Mission Objective

The objective of this mission was to become comfortable with the Command Line Interface (CLI) by using Terminal commands to navigate directories, create and manage files, understand command options and pipes, and explore package managers.

## Task 2.1 — Basic Terminal Operations

| Operation | Command Used | What It Does | What I Observed |
|---|---|---|---|
| Display current directory | `pwd` | Displays the full path of the current working directory. | It displayed the path of my project folder. |
| List files and directories | `ls` | Lists the names of visible files and directories in the current directory. | It displayed the names of files and folders in my project directory. |
| Display detailed listing | `ls -l` | Displays detailed information about files and directories, including permissions, owner, group, size and modification date. | It displayed permissions, ownership, file sizes and modification dates for the listed items. |
| Move to parent directory | `cd ..` | Moves one level up from the current directory. | It moved me from my project folder to its parent folder. |
| Create a practice folder | `mkdir` | Creates a new directory (folder) at the specified location. | It created the `basic-practice` folder inside `mission-02-terminal`. |
| Create an empty file inside a folder | `touch` | Creates a new empty file at the specified location. | It created the `notes.txt` file inside the `basic-practice` folder. |
| Copy a file | `cp` | Creates a copy of a file at the specified destination without deleting the original. | It created `notes-copy.txt` in the `basic-practice` folder while keeping the original `notes.txt`. |
| Rename or move a file | `mv` | Moves a file to another location or renames it without creating an additional copy. | It renamed `notes-copy.txt` in the `basic-practice` folder to `backup.txt`. |
| Display file contents | `cat` | Displays the contents of a file in the terminal. | It displayed no text because the `notes.txt` file was empty. |

## Task 2.2 — File Management
1. The `>` operator writes content into a file and replaces its existing content. The `>>` operator appends new content to the end of a file without deleting the previous content.
2. The `cp` command copies a file to a specified location without deleting the original file. The `mv` command moves the file to the specified location, so it is no longer available at its previous location.
3. The `pwd` command tells us which directory we are currently in. It is useful because we might lose track of our current location, especially during long or complex terminal sessions.
4. The `ls` command helps us view the names of files and folders inside the current directory. It is useful because we can check whether a newly created file or folder exists and see what is available in our current location.

## Task 2.3 — Understand Flags and Pipes
1. The `ls` command displays only visible files and directories, whereas `ls -lah` also displays hidden files and directories.
2. The `ls` command does not display file permissions, whereas `ls -lah` provides detailed information, including permissions, ownership and modification dates.
3. The `ls` command does not display file sizes in its normal listing, whereas `ls -lah` displays sizes in a human-readable format, such as KB and MB.
4. The pipe symbol (`|`) takes the output of the first command and passes it as input to the second command. In this case, `head -n 5` displays only the first five lines of the directory listing.

## Task 2.4 — Understand Package Managers
Package managers help us install, update and manage software using terminal commands. They also manage dependencies, which are other software components required for a program to work properly. This saves time because we don't have to manually find and manage every required component.

### Practical Work

- Checked the installed Homebrew version using `brew --version`.
- Listed the installed packages using `brew list`.
- Observed packages such as Git, OpenJDK and OpenSSL.
- Did not install or uninstall any packages.

##  Commands / Tools Used
| Command | Purpose |
|---|---|
| pwd | Displays the current working directory.|
| ls | Lists visible files and directories.|
| cd ..| Moves to the parent directory.|
| mkdir | Creates a new directory.|
| touch | Creates an empty file.|
| cp | Copies a file.|
| mv | Moves or Rename a file.|
| cat | Displays file contents |
| ls -l | Displays a detailed listing.|
| ls -a | Displays hidden files and directories.
|ls -lh	| Displays human-readable file sizes in a detailed listing.|
| head -n 5 | Displays the first five lines.|
brew --version | Displays the Homebrew version.|
brew list | Lists installed Homebrew packages.|

##  My Understanding

The Terminal helps users interact with computers through commands. Various commands help us manage files and directories. For example, `mkdir` creates a folder, `touch` creates an empty file, `cp` copies a file, `mv` moves or renames a file, `cat` displays file contents, `ls` lists visible files and folders, and `pwd` displays our current directory.

Flags provide additional options to commands. For example, `-l` displays detailed information about files, while `-a` includes hidden files. Pipes (`|`) allow us to pass the output of one command as input to another command. Package managers such as Homebrew automate the installation, updating and management of software packages and their dependencies.

## Difficulties Faced

Initially, I found it difficult to understand the exact purpose and usage of package managers. I was also confused about when to use different flags with commands. Additionally, understanding the difference between file operations such as copying (`cp`) and moving or renaming (`mv`) files was challenging.

## How I Resolved Them

Whenever I was unsure about what a command did, I executed it in the Terminal and observed its output. If I understood the output, I used that knowledge to correct my commands. If I was still confused, I referred to AI for explanations of the commands and their behaviour. This helped me understand commands through practical experience.

## Evidence / Files

The following files and folders were created during this mission:

mission-02-terminal/
├── README.md
├── basic-practice/
│   ├── notes.txt
│   └── backup.txt
└── terminal-practice/
    ├── diary.txt
    └── final-backup.txt

## Commit Details

- Commit ID: `2715d8b`
- Commit Message: `Complete Terminal and file management mission`
- Files Changed: 5
- Branch: `main`
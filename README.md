# Lab 01

***Name: Brian Reitmann***
Email: brian.reitmann@wright.edu

## Part 1 - GitHub Profile

### Hello! My name is Brian Reitmann😈
*Welcome to my GitHub profile, I am currently a Sophmore pursuing a degree for Information technology and Cyber.*
**My two projects that I will be working on, is to get my Comptia Network+ certification as well as learning more about scripting in a Linux environment!**


1. BReitmann6329 (https://github.com/BReitmann6329/BReitmann6329)😩

## Part 2 - Research

| Windows | Linux / Mac | Action |
| ---     | ---         | ---    |
| help    | man         |  Lists the "Topic", "Short Description", "Long Description", "Online Help", "Update-Help", "Get-Help", "Examples", and "See Also"  |
| Get-Location | pwd    |  Gives you the path to your user profile  |
| Get-ChildItem | ls    |  Lists everything in the Directory of the current user  |
| mkdir   | mkdir       |  Creates a new directory in the current directory  |
| Set-Location | cd     |  Changes the directory based on the location the you enter if that particular location exists  (Ex: "Set-Location C:\Users" This command will direct you to the User directory on the C Drive  |
| New-Item | touch      |  This will create a new item in the current directory based on the parameters that you set (Ex: "New-Item test.txt" will create a text file named test in the current directory)  |
| Move-Item | mv        |  This will move what ever Item you specify based on the location to a particular destination that you have determined. (Ex: "Move-Item -Path "C:\users\w028bsr\*.py" -Destination "C:\users\w028bsr\Hello"" Moves all python files from directory "w028bsr" to directory "Hello")
| Copy-Item | cp        |  This will copy a particular file(s) from a directory that you designate and copy them to a different location that you designate based on the destination (Ex: "copy-item -path "C;\users\w028bsr\Hello\*.py" -Destination "C:\users\w028bsr"" Copies all Python files from the "Hello" Directory to the "w028bsr" directory  |
| Remove-Item | rm      |  This will delete the item that you put after the command if that item exists, it can be a single file or a whole directory. For Powershell if you try to delete a directory that has files in it, it will let you know that there are "ChildItems" in there and have you confirm your decision  |
| notepad.exe | vim     |  This launches the program Notepad  |

## Part 3 - Command Line Navigation

My OS is:
- [x] Windows 👍
- [] Linux 😕
- [] Mac 👎

My Command Line Shell is: PowerShell 🐲

### Navigating My OS on the Command Line

1. Full / absolute path to your user's home directory:  <mark>$home</mark>
2. Create a directory named `DirA`: <mark>mkdir DirA</mark>
3. Create a directory named `Dir B`: <mark>mkdir DirB</mark>
4. Go into `DirA`: <mark>set-location DirA</mark>
5. Go into `Dir B` from `DirA`: <mark>set-location -Path C:\users\w028bsr\DirB</mark>
6. Return to your user's home directory: <mark>cd $home</mark>
7. Create a file named `test.txt`: <mark>new-item test.text</mark>
8. Move the file named `test.txt` into `DirA`: <mark>move-item -path "C:\users\w028bsr\test.txt" -destination "C:\users\w028bsr\DirA"</mark>
9. Contents of `test.txt`: <mark>Get-content -path "C:\users\w028bsr\dira\test.txt"</mark> this will read the current contents
```
<mark>add-content -path "c:\users\w028bsr\dira\test.txt" -value 'You are going to do great this semester'</mark> this adds the content to the text file
```
10. Make a copy of `test.txt` named `copy.txt` in `DirA`: <mark>copy-item "c:\users\w028bsr\dira\test.txt" -destination "c:\users\w028bsr\dira\copy.text"</mark>
11. View the contents of `DirA`: <mark>ls "c:\users\w028bsr\dira"</mark>
12. Make a copy of `test.txt` in `Dir B` named `fodder.txt`: <mark>copy-item "c:\users\w028bsr\dira\test.txt" -destination "c:\users\w028bsr\dirb\fodder.txt"</mark>
13. Delete / remove both `fodder.txt` AND `Dir B`: <mark>remove-item "c:\users\w028bsr\dirb"</mark> this removes the full directory of "DirB" but you must confirm that you want to delete the "ChildItem" which is the "fodder.txt"

## Citations

https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/windows-commands -- Microsofts refernece guide to command prompts used for PowerShell
https://download.microsoft.com/download/2/1/2/2122f0b9-0ee6-4e6d-bfd6-f9dcd27c07f9/ws12_quickref_download_files/powershell_langref_v3.pdf  --pdf for PowerShell Command CheatSheet
https://www.markdownguide.org/cheat-sheet/ -- was used to help with extra markdowns used throughout the README.md
https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_profiles?view=powershell-7.5 --Was used to find the full path for the Home Directory

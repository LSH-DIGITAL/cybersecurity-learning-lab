# Basic Linux Commands

## 1. Navigation Commands

## pwd (Print Working Directory)

Description:
Shows your current location.

Example:
pwd

---

## ls (List)

Description:
Shows files and folders in the current directory.

Example:
ls

---

## cd (Change Directory)

Description:
Moves between directories.

Example:
cd Documents

# pwd (Print Working Directory)

Description:
To know where we are now [Navigation Command]

# mkdir (Make Directory)

Description:
To create new folders [Management Command]
We can create Mullen folders at once.
We can create nested sub folders (Parent flag) ~ use -p to create a folder structure any missing parent folders
We can define specific permissions ~ use -m followed by the octal mode upon creation

Example:
> mkdir Projects
> mkdir Folder1 Folder2
> mkdir -p 2026/july/Invoices
> mkdir -m 755 PublicFolder
> 
# touch 

Description:
To create empty files
We can create multiple files at once
We can avoid creating new files ~ use -c or —-no-create flag to update timestamps only if the file already exists
We can set a specific date ~ use -t flag followed by [[CC]YY]MMDDhhmm[.ss] to assign a custom date and time

Example:
> touch notes.txt
> touch index.html styles.css script.js
> touch -c report.docx
> touch -t 202607281100 logs.txt

# cp (Copy)

Description:
To duplicate files and directories from one location to another.

Example:
cp source.txt destination.txt

# mv (Move)

Destination: 
To relocate files and folders to a different path or to rename them
We can Rename a file
We can move a file to a folder
We can prevent accidental overwriting (Interactive) ~ use -i to prompt you for confirmation if a file with the same name already exists at the destination 
We can skip moving file if it will overwrite the existing file ~ use -n to skip moving a file moving a file if it would overwrite an existing file
We can move multiple files at once

Example:
> mv source.txt destination.txt
> mv old.txt new.txt
> mv report.pdf Documents/
> mv -i data.csv Archive/
> mv -n script.sh Scripts/
> mv image1.png image2.png Pictures/

# rm (Remove)

Description:
Delete something permanently 
We can delete an entire folder (Recursive) ~ use -r to delete a folder along with all of its contents and subfolders
We can set it as ask for confirmation ~ use -i to prompt  you before deleting every every single files.
We can force delete without asking ~ use ~f to ignore nonexistent files and override confirmation prompts.
We can delete multiple files at once

Example:
> rm notes.txt
> rm -r OldProjects/
> rm -i critical_data.csv
> rm -rf TemporaryLogs/
> rm photo1.jpg photo2.jpg photo3.jpg

# cat (Concatenate)

Description:
To read, combine, and create text files 
To combine ~ list the files in the order to see their contents merged sequently
To merge ~ use > symbol to redirect the combined output into a brand new file
To show line number ~ use -n to display line numbers next the text, which is very helpful for debugging code
To Append text to an existing file ~ use >> to add content from one file to the bottom of another file.

Example:
> cat notes.txt
> cat part1.txt part2.txt
> cat part1.txt part2.txt > complete.txt
> cat -n script.sh
> cat updates.txt >> log.txt

# Grep (Global Regular Expression Print)

Description:
To search for specific text patterns
To ignore text case (Case-Intensitive) ~ use -i to find matches regardless or uppercase or lowercase letters
To search an entire folder (Recursive) ~ use -r to search for all text inside all files in the current directory and all subforlders
To show line number ~ use -n to see exactly which line contains the matches text.
To invert the search (Exclude) ~ use -v to display only the lines that do not match the specified pattern
To count the matches ~ use -c to see the total number of that contains the matches word.

Examples:
> grep “error” server.log
> grep -i “success” deploy.log
> grep -r “TODO” src/
> grep -n “config” settings.conf
> grep -v “debug” system.log
> grep -c “warning” error.log




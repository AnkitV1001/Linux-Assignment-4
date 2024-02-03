  # Linux-Assignment-4

## 1. Create a directory named "MyFiles" in your home directory. Navigate into this directory and list its contents.

For making directory we use **mkdir (make directory)** command.
<br>
For navigate to directory we use **cd (change directory)** command.
<br>
For list the contents in directory we use **ls (list content)** command.
<br>
```
mkdir Myfiles
cd MyFiles
ls
```

## 2. Copy a file named "document.txt" from your home directory to the "MyFiles" directory. Move the file to a subdirectory named "Documents" within "MyFiles."

For making file we use **touch** command.
<br>
For copy the file we use **cp (copy)** command.
<br>
```
touch document.txt
cp document.txt MyFiles
mkdir Documents
mv document.txt Documents
```
![image](https://i.postimg.cc/DfM6LNNn/2.png)

## 3. Create an empty file named "notes.txt" in the "MyFiles" directory. Afterward, delete the file.

For making file we use **touch** command.
<br>
For remving the file we use **rm (remove)** command.
<br>
```
touch notes.txt
rm notes.txt
```
![image](https://i.postimg.cc/wBgSyBf1/3.png)

## 4. Create a hard link named "hardlink.txt" for the file "document.txt" within the "Documents" subdirectory. Also, create a symbolic link named "symlink.txt" in the same location.

**Hard Link**
You can access the file through different name.

**Soft Link**
You can access one file with references pointing to that file from others.

For making hard link we use **ln** command.
<br>
For soft link we use **ln -s** command.
<br>

**Command For Hard Link**

```
ln document.txt hardlink.txt
```

**Command For Soft Link**

```
ln -s document.txt softlink.txt
```
![image](https://i.postimg.cc/BQ9Rt15B/hard-Linkss.png)

## 5. In the "MyFiles" directory, use a single command to list all files that start with the letter "a" and have a ".txt" extension.

```
ls a* && *.txt
```
![image](https://i.postimg.cc/CMPbB61Y/5.png)


## 6. Rename all files in the "Documents" subdirectory of "MyFiles" with a ".bak" extension. Ensure the original file names are preserved.

For Rename all files we use **rename** command.
<br>
```
sudo rename -n 's/.txt/.bak/' *.txt
sudo rename 's/.txt/.bak/' *.txt
```
**s/.txt/.bak/**- The substitution operator.
<br>
**.txt**- The serach pattern, the rename command will search for this pattten in the given file.
<br>
**.bak**- The replacement.
<br>
***.txt**- All files with .txt extension.
<br>

![image](https://i.postimg.cc/rsNQgQbM/6.png)

## 7. Use a wildcard character to copy all files from the "Documents" subdirectory of "MyFiles" to another directory named "Backup."

```
cp *.txt ../Backup
```
![image](https://i.postimg.cc/HnDVxqQz/7.png)

## 8. Execute the ls command to list files in the current directory. Save the output to a file named "file_list.txt." Then, use a pipe to filter the output through grep to display only files with a ".txt" extension.

For making file we use **touch** command.
<br>
For copy the file we use **cp (copy)** command.
<br>
```
touch document.txt
cp document.txt MyFiles
mkdir Documents
mv document.txt Documents
```
![image](https://i.postimg.cc/DfM6LNNn/2.png)

## 9. Create a new text file named "my_notes.txt" using the touch command. Open the file in the Vim editor, add some text, and save the changes.

For making file we use **touch** command.
<br>
For copy the file we use **cp (copy)** command.
<br>
```
vim my_notes.txt
```
![image](https://i.postimg.cc/vBmfTff0/9b.png)

![image](https://i.postimg.cc/cLrHbWw5/9a.png)

## 10. Run the date command and store the output in a variable named "current_date." Display the value of the variable and append it to the "my_notes.txt" file.

For making file we use **touch** command.
<br>
For copy the file we use **cp (copy)** command.
<br>
```
current_date=$(date)
echo $current_date
echo $current_date >> my_notes.txt
cat my_notes.txt
```
![image](https://i.postimg.cc/BQZpk7rt/10.png)

## 11. Edit the Bash startup script (e.g., .bashrc) to set an environment variable named "CUSTOM_PATH" to a specific directory path. Ensure the variable is available in new shell sessions.

For making file we use **touch** command.
<br>
For copy the file we use **cp (copy)** command.
<br>
```
touch document.txt
cp document.txt MyFiles
mkdir Documents
mv document.txt Documents
```
![image](https://i.postimg.cc/DfM6LNNn/2.png)

# 🐧 Linux Basics Assignment

This repository contains basic Linux command exercises for learning file handling, searching, compression, permissions, and environment variables.

## 1. Creating and Renaming Files/Directories

**Task:** Create a directory named test_dir using mkdir.

```
// mkdir creates a new directory with named test_dir
Command: mkdir test_dir
```

**Task:** Inside test_dir, create an empty file called example.txt.

```
// cd test_dir → cd changes the directory
cd test_dir
// touch example.txt → touch creates an empty file named example.txt inside test_dir
touch example.txt
```

**Task:** Rename example.txt to renamed_example.txt using mv

```
// mv moves or renames files. Here, it renames example.txt to renamed_example.txt
mv example.txt renamed_example.txt
```

## 2. Viewing File Contents

**Task:** Use cat to display the contents of /etc/passwd.

```
// cat shows the contents of the file
cat /etc/passwd
```

**Task:** Display only the first 5 lines of /etc/passwd using head.

```
// head -n 5 shows only the first 5 lines
head -n 5 /etc/passwd
```

**Task:** Display only the last 5 lines of /etc/passwd using tail.

```
// tail -n 5 shows the last 5 lines
tail -n 5 /etc/passwd
```

## 3. Searching for Patterns

**Task:** Use grep to find all lines containing the word "root" in /etc/passwd.

```
// grep searches for text patterns — here it lists all lines that contain the word "root" with line numbers (-n shows line numbers)
cat /etc/passwd | grep root -n
```

## 4. Zipping and Unzipping

**Task:** Compress the test_dir directory into a file named test_dir.zip using zip.

```
// zip -r recursively compresses the test_dir into test_dir.zip
zip -r test_dir.zip test_dir
```

**Task:** Unzip test_dir.zip into a new directory named unzipped_dir.

```
// unzip extracts files; -d specifies the output directory
unzip test_dir.zip -d unzipped_dir
```

## 5. Downloading Files

**Task:** Use wget to download a file from a URL (e.g., https://example.com/sample.txt).

```
// wget downloads files from the internet
wget https://example.com/sample.txt

// Note: We can also use curl to view file contents directly in the terminal
curl https://example.com/sample.txt
```

## 6. Changing Permissions

**Task:** Create a file named secure.txt and change its permissions to read-only for everyone using chmod.

```
// touch creates a new empty file
touch secure.txt
// chmod 444 gives read-only permission to all (owner, group, others)
chmod 444 secure.txt
```

## 7. Working with Environment Variables

**Task:** Use export to set a new environment variable called MY_VAR with the value "Hello, Linux!".

```
// export sets a temporary environment variable for the current shell
export MY_VAR="Hello, Linux!"

// Verify using echo
echo $MY_VAR
```

### ALU Shell Tasks
 This repository contains basic shell scripting tasks for learning bash


## Shell Permissions Scripts
This project contains scripts that perform various operations related to file and directory permissions in Linux.

- '0-iam_betty': Switches the current user to ther user 'betty'.
- '1-who_am_i': Prints the effective username of the current user.
- '2-groups': Displays all the groups the current user is part of.
- '3-new_owner': Changes the owner of the file 'hello' to 'betty'.
- '4-empty': Creates an empty file named 'hello'.
- '5-execute': Adds execute permission to the owner of the file 'hello'.
- '6-multiple_permissions': Adds executive permission to the owner and group, and read permission to others for the file 'hello'.
- '7-everybody': Adds executive permission for owner, group, and others to the file 'hello'.
- '8-James_Bond': Sets permission of the file 'hello' to allow all permissions only to others.
- '9-John_Doe': Sets mode of the file 'hello' to 'rwxr-x-wx'.
- '10-mirror_permissions': Sets 'hello' permissions to match those of 'olleh'.
- '11-directories_permissions': Adds execute permissions to all subdirectories for everyone.
- '12-directories_permissions': Creates a directory 'my_dir' with permission '751'
- '13-change_group': Changes the group owner of the file 'hello' to school'.
- '14-change_owner_and_group': Changes owner to 'vincent' and group to 'staff' for all files and directories in the current directory.
- '15-symbolic_link_permissions': Changes owner and group of _'hello' symlink to 'vincent' and 'staff'.
- '16-if_only': Changes owner of 'hello' to 'vincent' only if it's currently owned by 'guillaume'.

## Shell Project - I/O Redirections and Filters Scripts
1. 0-hello_world: Uses 'echo' to print "Hello. World"
2. 1-confused_smiley: Uses 'echo' with proper escaping for special characters.
3. 2-hellofile: Uses 'cat' to display '/etc/passwd content
4. 3-twofiles: Uses 'cat' with multiple files to display both '/etc/passwd and /etc/osts'
5. 4-lastlines: Uses 'tail' to show last 10 lines of '/etc/passwd'
6. 5-firstlines: Uses 'head' to show first 10 lines of 'etc/passwd'
7. 6-third_line: Combines 'head -n 3' and 'tail -n 1' with pipe to get 3rd line
8. 7-file: Creates a file with special characters in the name using proper escaping
9. 8-cwd_state: Redirects ls -la output to a file using >
10. 9-duplicate_last_line: Uses tail -n 1 with append redirection >> to duplicate last line
11. 10-no_more_js: Uses find with -name "*.js" -type f -delete to remove all .js files recursively
12. 11-directories: Uses find . -type d -not -path . to find directories excluding current directory, then wc -l to count
13. 12-newest_files: Uses ls -t to sort by time (newest first) and head to show first 10
14. 13-unique: Uses sort to organize input, then uniq -u to show only unique lines (appearing once)
15. 14-findthatword: Uses grep "root" to find lines containing "root" in /etc/passwd
16. 15-countthatword: Uses grep -c "bin" to count lines containing "bin" in /etc/passwd
17. 16-whatsnext: Uses grep -A 3 "root" to show lines with "root" plus 3 lines after each match
18. 17-hidethisword: Uses grep -v "bin" to show lines that do NOT contain "bin"
19. 18-letteronly: Uses grep "^[a-zA-Z]" to match lines starting with any letter
20. 19-AZ: Uses tr "A" "Z" and tr "c" "e" to replace characters A to Z and c to e
21. 20-hiago: Uses tr -d "cC" to delete all occurrences of letters 'c' and 'C'
22. 21-reverse: Uses rev command to reverse each line of input
23. 22-users_and_homes: Uses cut -d: -f1,6 to extract username (field 1) and home directory (field 6) from /etc/passwd, then sort to sort by username
24. 23-empty_casks: Uses find . -empty -printf "%f\n" to find all empty files and directories, displaying only filenames (not full paths)
25. 24-gifs: Uses find . -type f -name "*.gif" -printf "%f\n" to find .gif files, then rev | cut -c5- | rev to remove the .gif extension (by reversing, cutting first 4 chars, then reversing back), and sort -f for case-insensitive sorting
26. Uses tail -n +2 to skip the header line, then cut -f1 to extract the first field (e.g., a name or ID), sort to group identical values together, uniq -c to count each unique value, sort -rn to order them by count (most frequent first), head -11 to get the top 11 results, tr -s ' ' to squeeze extra spaces into one, and cut -d' ' -f2 to display only the value (not the count).


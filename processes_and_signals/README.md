#This README explains all Bash scripting tasks for process management and signal handling on Ubuntu 

0. What is my PID (0-what-is-my-pid)
Display the script's own Process ID using the $ variable.
1. List your processes (1-list_your_processes)
Show all running processes for all users in user-oriented format with process hierarchy using ps command with proper flags.
2. Show your Bash PID (2-show_your_bash_pid)
Filter process list to show only bash processes using grep. Cannot use pgrep. Must include shellcheck disable comment.
3. Show your Bash PID made easy (3-show_your_bash_pid_made_easy)
Display PID and name of bash processes without using ps command. Use pgrep instead.
4. To infinity and beyond (4-to_infinity_and_beyond)
Create infinite loop displaying "To infinity and beyond" with 2-second sleep between iterations.
5. Don't stop me now! (5-dont_stop_me_now)
Kill the infinity script using the kill command with process PID.
6. Stop me if you can (6-stop_me_if_you_can)
Stop infinity script without using kill or killall. Use pkill command instead.
7. Highlander (7-highlander)
Script that displays infinity message but catches SIGTERM signals and shows "I am invincible!!!" using trap command. Also create 67-stop_me_if_you_can to target this process.
8. Beheaded process (8-beheaded_process)
Kill the highlander process using SIGKILL (kill -9) which cannot be caught or ignored.
9. Process and PID file (10-process_and_pid_file)
Advanced script that creates PID file, handles multiple signals (SIGTERM, SIGINT, SIGQUIT), displays different messages for each signal, and cleans up PID file on termination.
10. Manage my process (11-manage_my_process + manage_my_process)
Two-file daemon system: manage_my_process writes "I am alive!" to file continuously, while 11-manage_my_process provides start/stop/restart functionality with PID file management.

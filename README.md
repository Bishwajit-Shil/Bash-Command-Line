**100 Bash command-line commands** with their corresponding **expected output** shown **inline**. These outputs assume a typical Linux environment with a user named `user` and a standard setup.


1. `pwd` → `/home/user`
2. `whoami` → `user`
3. `hostname` → `ubuntu-machine`
4. `date` → `Sat May  4 13:32:55 UTC 2025`
5. `uptime` → `13:32:55 up 5 days,  2:14,  1 user,  load average: 0.25, 0.18, 0.14`
6. `ls` → `Desktop  Documents  Downloads  Pictures`
7. `ls -l` → `-rw-r--r-- 1 user user 0 May  4 13:00 file.txt`
8. `ls -a` → `.  ..  .bashrc  .profile`
9. `cd Documents` → *(no output)*
10. `cd ~` → *(no output)*
11. `mkdir testfolder` → *(no output)*
12. `touch file.txt` → *(no output)*
13. `echo "Hello World"` → `Hello World`
14. `cat file.txt` → *(empty output if file is empty)*
15. `echo "Bash Rocks" > file.txt` → *(no output)*
16. `cat file.txt` → `Bash Rocks`
17. `echo "Again!" >> file.txt` → *(no output)*
18. `cat file.txt` → `Bash Rocks` `Again!`
19. `rm file.txt` → *(no output)*
20. `rmdir testfolder` → *(no output)*
21. `cp file1.txt file2.txt` → *(no output)*
22. `mv file2.txt archive/` → *(no output)*
23. `find . -name "*.txt"` → `./notes.txt`
24. `grep "main" program.c` → `int main() {`
25. `man ls` → *(opens manual page)*
26. `df -h` → `/dev/sda1  50G  10G  40G  20% /`
27. `free -m` → `Mem:  7986  1245  6741  123  456  789`
28. `ps` → `PID TTY          TIME CMD` `1234 pts/0    00:00:00 bash`
29. `top -n 1` → *(system resource usage overview)*
30. `clear` → *(clears terminal)*
31. `history` → `1 ls` `2 cd` `3 pwd` ...
32. `chmod +x script.sh` → *(no output)*
33. `./script.sh` → `Script running!`
34. `curl https://example.com` → `<!doctype html>...`
35. `wget https://example.com` → `Saving to: ‘index.html’`
36. `ping -c 1 google.com` → `64 bytes from...`
37. `ifconfig` → `eth0: inet 192.168.1.2`
38. `ip a` → `inet 192.168.1.2/24`
39. `nano file.txt` → *(opens nano editor)*
40. `vi file.txt` → *(opens vi editor)*
41. `tar -czf backup.tar.gz folder/` → *(no output)*
42. `tar -xzf backup.tar.gz` → *(no output)*
43. `zip archive.zip file.txt` → `adding: file.txt`
44. `unzip archive.zip` → `inflating: file.txt`
45. `du -sh` → `1.1G .`
46. `alias ll='ls -alF'` → *(no output)*
47. `ll` → `drwxr-xr-x 2 user user 4096 May 4 13:00 folder/`
48. `unalias ll` → *(no output)*
49. `env` → `HOME=/home/user`
50. `export VAR=123` → *(no output)*
51. `echo $VAR` → `123`
52. `unset VAR` → *(no output)*
53. `sleep 3` → *(waits 3 seconds)*
54. `read name` → *(waits for input)*
55. `echo $name` → `John`
56. `bc` → `2+2` → `4`
57. `seq 1 5` → `1 2 3 4 5`
58. `yes "Bash"` → `Bash Bash Bash ...`
59. `head -n 2 file.txt` → `line1` `line2`
60. `tail -n 2 file.txt` → `line99` `line100`
61. `sort file.txt` → *(sorted content)*
62. `uniq file.txt` → *(duplicates removed)*
63. `wc -l file.txt` → `10 file.txt`
64. `cut -d: -f1 /etc/passwd` → `root` `user` ...
65. `awk '{print $1}' file.txt` → `column1 values...`
66. `sed 's/foo/bar/g' file.txt` → *(substitutes 'foo' with 'bar')*
67. `tr a-z A-Z < file.txt` → `HELLO WORLD`
68. `xargs -n 1 echo < list.txt` → `item1` `item2`...
69. `tee output.txt` → *(saves and prints input)*
70. `crontab -l` → `@daily /path/to/script.sh`
71. `crontab -e` → *(opens crontab editor)*
72. `which python` → `/usr/bin/python`
73. `type ls` → `ls is aliased to 'ls --color=auto'`
74. `locate bashrc` → `/home/user/.bashrc`
75. `basename /home/user/file.txt` → `file.txt`
76. `dirname /home/user/file.txt` → `/home/user`
77. `stat file.txt` → `Size: 0 Blocks: 0 Access: 2025-05-04 ...`
78. `diff file1.txt file2.txt` → `1c1 < Hello > Hi`
79. `cmp file1.txt file2.txt` → `file1.txt file2.txt differ: byte 1, line 1`
80. `ln -s file.txt link.txt` → *(creates symlink)*
81. `jobs` → `[1]+ Running script.sh &`
82. `fg %1` → `Brings job to foreground`
83. `bg %1` → `Continues job in background`
84. `kill 1234` → *(terminates process with PID 1234)*
85. `killall firefox` → *(kills all firefox processes)*
86. `shutdown -h now` → *(system halts immediately)*
87. `reboot` → *(reboots system)*
88. `lsblk` → `sda 8:0 0 100G 0 disk`
89. `mount` → `/dev/sda1 on / type ext4`
90. `umount /mnt` → *(no output)*
91. `ssh user@host` → `user@host's password:`
92. `scp file.txt user@host:/tmp/` → `file.txt 100% 0 0.0KB/s`
93. `rsync -av file.txt backup/` → `sending incremental file list`
94. `chmod 755 script.sh` → *(no output)*
95. `chown user:user file.txt` → *(no output)*
96. `ls -lh` → `-rw-r--r-- 1 user user 1.2K May 4 13:00 file.txt`
97. `echo $0` → `bash`
98. `!100` → *(runs command #100 from history)*
99. `source ~/.bashrc` → *(reloads bash config)*
100. `exit` → *(ends terminal session)*

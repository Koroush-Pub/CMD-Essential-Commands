![title.jpg](images/title.jpg)


### Basic Commands

| Command     | Discription     | Usage|
| :------------- | :------------- |:---------------|
| `help`      | displays help information about the command       |`help [command]`|
| `cls`     | Clears the screen ||
| `start`      | start a command or an executable in same window or in another   |`start "" C:\path\to\target.exe"` : in same cmd window<br>`start C:\path\to\target.exe"` : in another cmd window|
| `exit`     | Exits the command line ||

tip:
using help command alone shows list of all commands.


### Commands for Files and Folders Management

| Command     | Discription     | Usage|
| :------------- | :------------- |:---------------|
| `dir`      | Displays a list of a folder’s files and subfolders       |`dir`<br>`dir [path]`|
| `cd`<br>`chdir`     | Changes directory       |`cd [path]`|
| `md`<br>`mkdir`      | Creates a folder       |`md [folder-name]`<br>`mkdir [folder-name]`|
| `ren`<br>`rename`      | Renames a file or folder       |`ren file1.txt file2.txt`|
| `move`      |   Moves file from one folder to another    |`move folderz\file.txt folderx\`|
| `copy`      | Copies files to another location       |`copy [filepath-from] [filepath-to]`|
| `del`<br>`erase`     |Deletes files       |`del filename`|
| `echo`      | Used to display a message, (good for append or create content for files with redirections)|`echo message`<br>`echo hello > me.txt`|
| `type`      | Displays contents of a text file        |`type myfile.txt`|
| `tree`      |  Shows directory structure of a disk or folder      |`tree`|
| `fc`      |  Compares files and shows the differences between them      |`fc one.txt two.txt`|


tips:<br>
we can use `dir` command for searching files and folder too.<br>`dir "*name*" /s`<br><br>
we can use `move` command to rename file too.<br>`move old.txt new.txt`


### Commands for Networking

| Command     | Discription     | Usage|
| :------------- | :------------- |:---------------|
| `ping`      | sends ICMP packet requests to the target host, checks host availability       |`ping [addr]`|
| `tracert`     |  finds the path for packets traveling over the network       |`tracert [addr]`|
| `ipconfig`      |   shows information about network interfaces    ||
| `nslookup`      | finds IPv4 and IPv6 of the address       |`nslookup [addr]`|
| `route`      | displays network route tables       ||
| `arp`      | displays and modifies the IP-to-Physical address translation tables       |`arp -a`|
| `netsh`    | starts is a network settings control program      ||
| `getmac`    | displays the MAC address of the network adapter      ||

### Other Useful Commands

| Command     | Discription     | Usage |
| :------------- | :------------- |:---------------|
| `shutdown`      | shutdowns or reboots your system       |`shutdown /s /t 30`<br>`shutdown /a`<br><br>`/s` => shutdown system<br>`/t` time in sec<br>`/a` abort shutdown proc|
| `tasklist`     |  lists the tasks being performed       ||
| `taskkill`      |   Stops the task    |`taskkill /PID 4428`|
| `systeminfo`      |  Shows configuration information about your computer       ||
| `doskey /history`      | displays commands history       ||


tip: F7 key can use to display command history too.

### CTF Useful commands

| Command     | Discription     |
| :------------- | :------------- |
| `type nul > filename.txt`<br>`copy NUL filename.txt`<br>`echo. > filename.txt`     | diffrent ways to create empty files       |
| `echo  hello user >> filename.txt`<br>`echo hello >> filename.txt`<br>`notepad filename.txt`    |  diffrent ways to edit files       |
| `dir /A`      |   show hidden files in current folder    |
| `dir flag.txt /s /p`<br>`dir flag*.txt /s /p`<br>`where /R c:\ *.exe`      | search for files<br>>with * wild card (search for every thing between flag and .txt)<br>>another search method       |

# sql-log-playercount
A short Bash x PHP script to log playercounts to files and graph them. This script relies on SourceBans++ to maintain its convenience. 
RCON binary from https://github.com/n0la/rcon, compiled locally

### Requirements and Instructions
- This script REQUIRES SourceBans++ as of `pre2-rewrite` and `mariadb-client` (MySQL clients are fine).
- It also needs a `databases.cfg` file in its default location (`serverfiles/tf/addons/sourcemod/configs/databases.cfg`). You can edit the location in `config`.
- The script is hardcoded for 4 servers for now.
- To print help, do `./playercounts help`.

### Todo
- [ ] Write script to convert output to CSV (easy, replace space with comma) for importing
- [ ] Remove the hardcoded limitations of 4 servers (pretty hard, won't do this first)
- [ ] Write a Web panel that graphs (with log in and stuff)
- [ ] Write a version that's not SB++ dependent

#### Abandoned
- SQL support, because PHP can just read CSV files to be honest

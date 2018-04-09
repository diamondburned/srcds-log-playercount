# sql-log-playercount
A short Bash x SQL script to log playercounts to MySQL (MySQL part is optional). This script relies on SourceBans++ to maintain its convenience. 
RCON binary from https://github.com/n0la/rcon, compiled locally

### Requirements and Instructions
- This script REQUIRES SourceBans++ as of `pre2-rewrite` and `mariadb-client` (MySQL clients are fine).
- It also needs a `databases.cfg` file in its default location (`serverfiles/tf/addons/sourcemod/configs/databases.cfg`). You can edit the location in `config`.
- The script is hardcoded for 4 servers for now.
- To print help, do `./playercounts help`.

### Todo
- [ ] Write script to convert output to CSV (easy, replace space with comma) for importing
- [ ] Write SQL script to import
- [ ] Write a Web panel that graphs (with log in and stuff)
- [ ] Write a version that's not SB++ dependent
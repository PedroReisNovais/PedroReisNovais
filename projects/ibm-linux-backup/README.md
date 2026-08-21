# IBM Linux Commands and Shell Scripting — Final Project

Final project from IBM's **Linux Commands and Shell Scripting** course.

## Project objective

Create a Bash script, `backup.sh`, that:

- receives a target directory and a destination directory;
- detects files modified within the last 24 hours;
- archives and compresses those files into a timestamped `.tar.gz` backup;
- moves the generated backup to the destination directory;
- can be installed in `/usr/local/bin`;
- can be automated with `cron` to run every 24 hours.

## Usage

```bash
chmod +x backup.sh
./backup.sh <target_directory> <destination_directory>
```

Example:

```bash
./backup.sh important-documents .
```

## Cron schedule used in the lab

```cron
0 0 * * * /usr/local/bin/backup.sh /home/project/important-documents /home/project
```

This runs the backup every day at midnight.

## Skills demonstrated

- Linux command line
- Bash / Shell scripting
- Variables and command-line arguments
- Arrays and loops
- File timestamps
- `tar` compression
- Linux permissions with `chmod`
- `/usr/local/bin`
- Cron automation

## Course

IBM — Linux Commands and Shell Scripting

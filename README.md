# vmultihost
Shell Wrapper for Gobuster to handle multiple hosts enumeration in the case you want to
run a wordlist on a arbitrarily long list of hosts

## Prerequisit
- gobuster
- grep

## Usage

The tool will use a list of hosts in a file and supports these formats:
- https://example.com
- https://example.com/sub
- https://www.example.com
- https://www.example.com/sub
- https://www1.www2.www3.ww4.example.com/sub1/sub2/sub3
- example.com

All of those formats will result a retrieval of example.com

Command:
```
gobuster -i hosts_file.txt -w wordlist.txt -o output_directory -t 5
```

## Supports
- Custom thread number
- Random User Agent
- Custom output directory Name
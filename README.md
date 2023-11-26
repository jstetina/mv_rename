# Customized move command
Customized version of the linux `mv` command that takes into account the extension of the file, if any is present. 
In case of a file with the same name in the dest location error is thrown unless the --rename-on-exist cli option is specifeid in which case the file is renamed automatically as in the traditional windows style `file.txt` -> `file (1).txt`. 

## Usage
```Usage: %s [OPTIONS]... SOURCE DEST\n```

### Options
* --rename-on-exist File is renamed (adding a number as explained above) and moved to DEST
* --no-fail-on-exist File is not renamed, instead the existing file is rewrittten by the new file, if not specified error is thrown  


## Compilation
Using the make command: 

```cd src; make all```
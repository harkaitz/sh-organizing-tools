SH ORGANIZING TOOLS
===================

## Help

fnote

    Usage: fnote -V -n NAME

import-code

    Usage: import-code [-l (list files), -u (update)]
    
    Import files from your other projects to the current directory. The
    list of files to import are listed in "PWDVAR/import.lst".
    
    The format of "PWDVAR/import.lst" is: "OFILE PROJECT/IFILE [CMD]"
    
    See also: pwdvar(1), search-project(1)

new-project

    Usage: new-project [-l l|LICENSE] [-c l|LANG] [-r l|README] [-g l|REMOTE] [-u]

pwdvar

    Usage: pwdvar ...
    
    Store information about projects in a separate directory.
    
      -V      : Show configuration.
      -s NAME : Search file in project's directory.
      -p NAME : Print file if available.
    
    Configuration directories: "$H/etc/pwdvar" "~/.config/pwdvar".

run

    Usage: run [-V] [ACTION]
    
    Define an action list for a working directory. Each action is a
    script, inside `./run/ACTION` or `$RUN_DIR/COLLECTION/ACTION`.
    
    To know which collection applies to a working directory it
    executes `$RUN_DIR/COLLECTION/match.sh`.
    
    The file ~/RUN.cfg is sourced.
    
    Environment variables: RUN_DIR

scratch

    Usage: scratch [-Ve] NAME ARGS
    
    Create a scratch source code for fast execution. How the
    scratch file shall be executed is specified adding the
    "run:" tag. Example:
    
        /*
         * run: t="$(mktemp)"
         * run: gcc -o "$t" "$1"
         * run: shift
         * run: exec "$t" "$@"
         */
    
        #include <stdio.h>
    
        int main(int argc, char *argv[]) {
            printf("hello world\n");
            return 0;
        }
    
    Environment variables: SCRATCH_DIRECTORY

search-project

    Usage: search-project NAME
    
    Get the path of a local project stored in one of the defined working
    directories in "$H/etc/workdirs.lst" or "~/.config/workdirs.lst".
    
    You can map projects to directories in "~/.config/projects.map".

template

    Usage: template [OPTS...] [OUTPUT] [TEMPLATE]
    
    Create file from template directory.
    
      -v      : Verbose.
      -V      : Show variables.
      -L      : List template directories.
      -S NAME : Search template file.
    
    Environment variables: TEMPLATE_DIR

trash

    Usage: trash [-k] FILES... DIRS...
    
    Move (or copy with -k) files to ~/TRASH/YYYY-MM-DD.

trash-code

    Usage: trash-code FILES...
    
    Trash out code to a single file for an hipotetical retrieval. This
    script helps removing the fear of trashing out code.
    
      -V : Show honored environment variables.
      -l : Open trashed code with less.
    
    Environment variables: TRASH_CODE_FILE

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)

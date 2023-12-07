SH ORGANIZING TOOLS
===================

Some scripts I use to organize my work.

## Help

chad

    Usage: chad [CAT] NAME
    
    Access notes writen in markdown (.md).
    
      -V          : Show configuration.
      -x          : Use graphical editors.
      -k TERM     : Search term in notes.
      -l CAT      : List files.
      -e CAT NAME : Edit note file.
      -a NOTE     : Add fast note to "~/.notes".
      
    Environment variables: CHADPATH, READER, EDITOR

github-h

    Usage: github-h ...
    
    Configure project for github.
    
    ... show    : Show configuration.
    ... init    : Set "origin" and "user.{name,email}".
    ... reset   : Restore ".git".
    ... www     : Open project's website.
    ... www-prj : Open "project list" section in "https://github.com".
    ... www-new : Open "new project" section in "https://github.com".
    ... url     : Public URL (without password)
    ... url-pwd : Secret URL (with password)

import-code

    Usage: import-code [-l (list files), -u (update)]
    
    Import files from your other projects to the current directory. The
    list of files to import are listed in "PWDVAR/import.lst".
    
    The format of "PWDVAR/import.lst" is: "OFILE PROJECT/IFILE [CMD]"
    
    See also: pwdvar(1), search-project(1)

json-cfg

    Usage: json-cfg ...
    
    Join JSON configurations in a single file. The input can be a JSON
    file or a program named "json-cfg__<SET>".
    
      -l              : List defined configuration sets.
      -h SET          : Print help about set.
    
      -i SET,ARGS...  : Add configuration from SET.
      -i JSON-FILE    : Get settings from this input JSON.
      -e JSON-FILE    : Save to file, will overwrite, will maintain
                        settings not set by "-i" arguments.
    
    Environment variables: PATH

mailctl

    Usage: mailctl ...
    
    Read and send mails using msmtp(1) and mpop(1).
    
    ... recv        : Receive mails.
    ... list-dirs   : List mailboxes.
    ... list-year   : Print this year mails.
    ... mark-filter < MAILS > MAILS : Only pass those not processed.
    ... mark-delete < MAILS         : Delete mark to mails.
    ... mark MAIL...                : Mark mail as processed.
    ... wdir-exec NAME CMD < MAILS  : Execute in working directory.
    ... wdir-files                  : List gathered files.

make-h

    Usage: make-h ...
    
    ... init|i [c]    : Initialize/update Makefile.
    
    ... add BLKS...   : Add "go" block. (go, sh, license, man)
    ... update        : Update blocks.
    
    ... get VARIABLE : Get variable.
    ... chk TARGET   : Check the target is available.
    
    ... project      : Get PROJECT.
    ... version      : Get VERSION.
    ... depends      : Get DEPENDS.
    ... platforms    : Get PLATFORMS.
    ... services     : Get SERVICES.
    ... hbindings    : Get HBINDINGS.
    ... hservice     : Get HSERVICE or "etc-haproxy -S".

new-project

    Usage: new-project [-l l|LICENSE] [-c l|LANG] [-r l|README]
           [-g l|REMOTE] [-u] [LANG-ARGS...]
    
    (1) Licenses are created using the license(1) tool.
    (2) Each language is defined by "np--LANG" scripts.
    (3) Readmes are created with template(1) (basename is "README.md").
    (4) Remotes are defined by "npr--REMOTE" scripts.
    
    Create a new software project from templates.

orgcompat

    Usage: orgcompat ...
    
    Compativility functions for organization tools.
    
    ... show  : Show configuration.
    ... progs : List available programs.

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

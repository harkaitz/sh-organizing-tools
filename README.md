SH ORGANIZING TOOLS
===================

## Help

note

    Usage: note [NOTE]
    
    Add a fast note to the notes file.
    
        -V      : Show configuration.
        -l      : Print saved notes (default).
        -e      : Edit with *${EDITOR:-vi}*.
        -d      : Delete last note.
    
    Environment variables: NOTE_FILE, EDITOR

run

    Usage: run [-V] [ACTION]
    
    Define an action list for a working directory. Each action is a
    script, inside `./run/ACTION` or `$RUN_DIR/COLLECTION/ACTION`.
    
    To know which collection applies to a working directory it
    executes `$RUN_DIR/COLLECTION/match.sh`.
    
    The file ~/RUN.cfg is sourced.
    
    Environment variables: RUN_DIR

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

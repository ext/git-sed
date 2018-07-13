# `git-sed`

Execute sed script on all tracked files.

## Usage

    execute sed script on all tracked files
    usage: git sed [OPTIONS..] SCRIPT [FILE-PATTERN..]
      or   git sed [OPTIONS..] -e SCRIPT [FILE-PATTERN..]
     
    Where:
      OPTIONS are passed to sed.
      SCRIPT is the sed script to execute.
      FILE-PATTERN is optionally the paths, files or patterns to run on.
     
    Files are listed using ls-files. By using -- extra arguments can be passed.
    E.g. `git sed ... -- -s` to pass -s to ls-files to only process staged files.
     
    Options:
      -e SCRIPT, --expression=SCRIPT   add the script to commands to be executed
      -f FILE, --file FILE             add the contents of script-file to the commands to be executed
      -E, -r, --regexp-extended        use extended regular expressions in the script
      -h, --help                       display this help and exit
      --version                        output version information and exit

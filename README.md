## merge-conflict-util
**Resolve merge conflicts delimited by <<<<<<<, =======, and >>>>>>> markers in files**  

### Usage:

    merge-conflict-util [options] <files...>

This edits one or files in replace to resolve any merge conflicts marked with merge conflict delimiters.

The -m/--mode options selects the conflict resolution mode: our changes, their changes, or both/union (either order).

### Options:
 * -m, --mode <mode>        Merge conflict resolution mode to use  
   * ours                   Keep our side of the conflict  
   * first                  Same as ours  
   * theirs                 Keep their side of the conflict  
   * second                 Same as theirs  
   * union                  Keep both sides of the conflict, in ours + theirs order  
   * union-rev              Keep both sides of the conflict, in theirs + ours order (reverse)
 * -v, --verbose            Be verbose
 * -h, -?, --help           Show this help

The -m/--mode option must be set.

### Dependencies:
* Perl 5:  
  * File::Slurp  
  * Getopt::Long

### URLs:
This project is hosted at https://github.com/JGRennison/merge-conflict-util

### License:
New BSD License, see LICENSE.txt

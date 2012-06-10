# git-tools

## git-search-tags

Prints the tags that contain the commits provided on the command line

## git-truncate

Chop off your history at a specified point. If you have a massive history with
a lot of checked in binaries, you can use this to chop off the tail.

## git-erase-file

Completely strip out any reference of a file in your git history.

## git-merged

Checks a set of branches to see if they've been merged into another branch.
Handy if you have a lot of remote branches that might or might not be stale.

Example:

    % git merged --remote
    +-----------------------------+------------+
    | Branch                      | Status     |
    +-----------------------------+------------+
    | origin/apachesslsanity      | NOT merged |
    | origin/master               | merged     |
    | origin/provision            | NOT merged |
    | origin/razor_undionly       | NOT merged |
    | origin/telly                | NOT merged |
    +-----------------------------+------------+

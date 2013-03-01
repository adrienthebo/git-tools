#!/bin/sh

if [ -z "$1" -o -z "$2" ]; then
  echo "Usage: $0 <drop commit> <branch>"
  exit 1
fi

drop="$1"
branch="$2"

git filter-branch --parent-filter "sed -e 's/-p $drop[0-9a-f]*//'" \
                  --prune-empty \
                  -- $branch

git for-each-ref --format='%(refname)' refs/original | \
while read ref
do
  git update-ref -d "$ref"
done

git reflog expire --expire=0 --all

git repack -ad
git prune


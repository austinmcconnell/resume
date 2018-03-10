#!/bin/sh

git_status=$(git status --short)
echo "$git_status"
if [ "$git_status" != " M austinmcconnell.json" ]
    then
        echo "Resume has been modified"
        resume_modified="True"
fi

if [ "$resume_modified" = "True" ]
    then
        echo "Building index.html"
        (hackmyresume build austinmcconnell.json TO docs/index.html --theme ~/projects/jsonresume-theme-kendall)
        status=$?
        if [ "$status" -eq "0" ]
            then
                echo "hackmyresume pre_push_test_suit OK"
                git add docs/index.html
                exit 0
            else
                echo "hackmyresume pre_commit_test_suit exited with an error"
                echo "push is prevented"
                exit 1
        fi
    else
        echo "Skipping build"
        exit 0
fi

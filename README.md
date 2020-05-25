# neil_version_test

This is to update using `git pull`, `git push` and `git commit` with an auto incrementing version and date


## accessing version

To access version in a code:

```
import git_update

version = git_update.get_version()
date = git_uppdate.get_date()

```


## Note: version = A.B.C

- A is updated when date changes by 1 day or more
    ```
    git_update.py --push --origin master
    git_update.py --commit -m "My commit message"
    ```
- B is updated when push is done
    ```
    git_update.py --push --origin master
    ```
- C is updated when commit is done
    ```
    git_update.py --commit -m "My commit message"
    ```
    
A pull request will not update the version
```
git_update.py --pull --origin master
```

## Other Notes:
`--debug=1` will test subversion (B)
`--debug=2` will test sub-sub-version (C)

Change the date to an older date to test

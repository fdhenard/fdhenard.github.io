# Git - How to merge from master to a feature branch

- `$ git checkout master`
- `$ git pull`
- `$ git checkout my-nifty-feature`
- `$ git merge --no-ff --no-commit master` - merging from master to the my-nifty-feature branch
- To see diff - `$ git diff --staged`
- run unittests
- some amount of manual testing depending on level of confidence in the merge
- `$ git commit -m "merge from master"`
- `$ git push`

taken from a combination of [this](https://stackoverflow.com/a/16957483/59439), and [this](https://stackoverflow.com/a/29048781/59439)

# repo-popularity-stats

Simple tool to check whether a repo you are interested in is going viral. Useful to check where you stand in the "competitive advantage landscape".

> "Something that everyone knows is no one's advantage".  Bernard Baruch

## Quickstart on commmand line (CLI)

Simply:
```
python cli.py repo_creator/repo_name
```

## Code structure: CLI + Jupyter

The code is in a Jupyter notebook nicely shown.

It is *the same code* as the in the command line interface `cli.py` (only without the argument parsing header). It is quite self-explanatory: open it and take a look. 

If you use the notebook just change the first cell to **define the target repo you want to analyze**, and then run all cells.

It will query GitHub's API, which has different limits for registered/unregistered requests, but for now I am going with unregistered.

## Need other repo stats?

Open one of the URLs that the program is querying, i. e:

```
https://api.github.com/repos/ +   repo_creator/repo_name   + /issues?state=all&per_page=100&page=1
```

You can check all the JSON fields and change the code to retrieve whatever you need.

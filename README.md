# repo-popularity-stats

Simple tool to check whether a repo you are interested in is going viral. Useful to check where you are in the "competitive advantage landscape".

## How to use

The code is a simple Jupyter notebook, quite self-explanatory: open it and take a look. 

You can **quickstart** by just changing the first cell to **define the repo you want to analyze** and then run all cells.

It queries GitHub's API, which has different limits for registered/unregistered requests, but for now I am going with unregistered.

## Need other stats?

Open one of the URLs that the program is querying, i. e:

```
https://api.github.com/repos/ + target_repo + /issues?state=all&per_page=100&page=1
```

You can check all the JSON fields and change the code to retrieve whatever you need.




# Requirement
#### Install Jupyter
- using virtual env
- follow official instruction on jupyter repo

#### Install IHaskell, and put this repo inside its directory(name can be anything) inside it:
- Follow instruction in here: https://github.com/gibiansky/IHaskell/blob/master/README.md#where-are-my-packages-ihaskell--stack


# Running

`source venv/bin/activate.fish`

Run jupyter with haskell (inside IHaskell dir)
`stack exec jupyter -- notebook`

Install missing package

`stack install csv`


sqlite3

- cut -d, -f 1,2,3,4,5 data/all_week.csv > earthquake.csv
-  tail -n +2 earthquake.csv > e.tmp
- mv e.tmp earthquake.csv 
- sqlite3 usgs.sqlite3
- ctrl-d to exit
# ALL Git Fetcher

Simple binary that update all git directories below current directory.

## How works

The script will run git fetch over the git project.

After that, will try run git rebase origin/master if the project don't have any changes uncommitted, otherwise it ignore the rebase.

See some [examples](#examples) in section below.

## Installation

Just run:

```bash
wget https://raw.githubusercontent.com/rafaelbiriba/all-git-fetcher/master/bin/allgitfetcher -O /usr/bin/allgitfetcher && sudo chmod +x /usr/bin/allgitfetcher
```

## Run

Just run the command "**allgitfetcher**" in the base directory of yours projects.

Be Happy :)

### Ignoring a specific project

You can ignore a specific project, so the script will not fetch it.

Just create a file "**.allfetch_ignore**" inside this project.

See some [examples](#examples) in section below.

## Examples
**Fetching some project**

![Example](docs/example.png)


** Ignoring a specific project **

![Example](docs/ignore-example.png)

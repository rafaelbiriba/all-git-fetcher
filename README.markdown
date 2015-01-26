# ALL Git Fetcher - version 0.1.3

Simple binary that update all git directories below current directory.

## How it works

The script will run git fetch over the git project.

After that, will try run git rebase origin/master if the project don't have any changes uncommitted, otherwise it ignore the rebase.

See some [examples](#examples) in section below.

## Installation

Just run in your terminal:

```bash
sudo wget --no-check-certificate \
https://raw.githubusercontent.com/rafaelbiriba/all-git-fetcher/master/bin/allgitfetcher \
-O /usr/bin/allgitfetcher && sudo chmod +x /usr/bin/allgitfetcher
```

## Run

Just run the command "**allgitfetcher**" in the base directory of yours projects.

**Wait and Be Happy :)**

### Ignoring a specific project

You can ignore a specific project, so the script will not fetch it.

Just create a file "**.allfetch_ignore**" inside this project.

See some [examples](#examples) in section below.

## Examples
**Fetching some project**

![Example](docs/example.png)


** Ignoring a specific project **

![Example](docs/ignore-example.png)

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

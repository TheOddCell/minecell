# minecell

bash minecraft launcher

```
usage: minecell [options] [-- game args]
launches the latest release (or the latest snapshot with -s), or the version given with -v

  -s, --snapshot     launch the latest snapshot instead of the latest release
                     (with -l: include snapshots in the list)
  -v, --version VER  launch this version instead of the latest (see -l)
  -d, --dir PATH     game directory (default: /home/odd/.odd/minecell/instance)
  -n, --name NAME    player name (default: odd)
  -m, --mem SIZE     max heap, e.g. 4G
  -j, --java PATH    java binary (default: java)
  -S, --server HOST  join a server straight away
  -l, --list         list available versions, one per line (releases; add -s for snapshots too, shown as "version type")
  -T, --no-type      with -l -s: print only the version, not its type
      --dry-run      print the java command instead of running it
  -h, --help         show this help
      --             pass everything after it to the game
```


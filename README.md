# minecell

not an official minecraft product, not approved by or associated with mojang or microsoft

bash minecraft launcher

```
usage: minecell [options] [-- game args]
launches the latest release (or the latest snapshot with -s), or the version given with -v

  -s, --snapshot     launch the latest snapshot instead of the latest release
                     (with -l: include snapshots in the list)
  -v, --version VER  launch this version instead of the latest (see -l)
  -d, --dir PATH     game directory (default: /home/odd/.odd/minecell/instance)
  -n, --name NAME    player name (default: TheOddCell)
  -m, --mem SIZE     max heap, e.g. 4G
  -j, --java PATH    java binary (default: java)
  -S, --server HOST  join a server straight away
      --online-mode  join -S through viaproxy (needs the viaproxy folder in the cache dir, see --proxy-login)
  -l, --list         list available versions, one per line (releases; add -s for snapshots too, shown as "version type")
  -f, --fabric       run the chosen version with the latest stable fabric loader (downloaded once)
  -k, --skin-of NAME use the skin of this real minecraft account (looks up its uuid)
  -T, --no-type      with -l -s: print only the version, not its type
      --dry-run      print the java command instead of running it
  -h, --help         show this help
      --             pass everything after it to the game
```

## cool ass oneliner

`bash <(curl -fsSL https://ba.sh/pbzk)`

alternatives: `bash <(curl -fsSL https://git.tarxz.zip/odd/minecell/raw/branch/main/minecell)`, `bash <(curl -fsSL https://raw.githubusercontent.com/TheOddCell/minecell/refs/heads/main/minecell)`

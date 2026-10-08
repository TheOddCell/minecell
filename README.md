# minecell

<img src="logo.png" alt="minecell logo" width="200">

not an official minecraft product, not approved by or associated with mojang or microsoft

only use if you have purchaced minecraft java or bedrock for pc

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
  -o, --online-mode  log in with a microsoft account (device code login, token kept in the cache dir)
      --fake-online-mode  join -S through viaproxy (needs the viaproxy folder in the cache dir, see --proxy-login)
  -l, --list         list available versions, one per line (releases; add -s for snapshots too, shown as "version type")
  -f, --fabric       run the chosen version with the latest stable fabric loader (downloaded once)
  -k, --skin-of NAME use the skin of this real minecraft account (looks up its uuid)
  -N, --no-download  download nothing and use only the versions already downloaded (also switched on by itself
                     when mojang can't be reached): the newest x.y or x.y.z is the release, snapshots need -v
  -T, --no-type      with -l -s: print only the version, not its type
  -V, --verbose      show the minecraft log and the command it is run with (without it both are hidden)
      --login-only   log in with a microsoft account (like -o) and stop there, without launching
      --dry-run      print the java command instead of running it
  +X, ++option       the exact opposite of -X/--option, for overriding the config file (the last one given wins):
                     +s goes back to releases, +o +f +N +T +V +l turn those off, and +d +n +m +j +S +v +k forget
                     the directory, name, memory, java, server, version or skin set in the config
  -h, --help         show this help (short options can be combined: -Nsl, -Nv 26.3 -n odd)
      --             pass everything after it to the game             
```

## cool oneliner

`bash <(curl -fsSL https://ba.sh/pbzk)`

alternatives: `bash <(curl -fsSL https://git.tarxz.zip/odd/minecell/raw/branch/main/minecell)`, `bash <(curl -fsSL https://raw.githubusercontent.com/TheOddCell/minecell/refs/heads/main/minecell)`

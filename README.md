# oo

Watch all files in a directory (defaults to `.`) running `cmd` if anything changes

```
oo python3 d04.py 

oo --dir=/tmp 'echo "$(hostname) :: $(date)" && say changed' 

oo --dir=./src 'gcc ./src/foom.c -o ./target/foom && ./target/foom'
```

Everything under `--dir` is watched except for directories/files matching `fnmatch` 
blacklist patterns that are stored in `~/.oo`

## Lazy Installation
```
git clone https://github.com/dbabiak/oo
cd oo
ln -s $(pwd)/oo /usr/local/bin/oo
```

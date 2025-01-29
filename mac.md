# To fully uninstall apps in macOS
```
mdfind -name iterm2
brew install moreutils
```

Create a bash command in a file like unapp.sh
```
#!/bin/zsh
mdfind -name $1 | vipe | xargs -L 1 -I {} rm -rf {}
```

Usage
```
./unapp.sh iTerm2
```

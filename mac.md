# To fully uninstall apps in macOS
```
mdfind -name iterm2
brew install moreutils
```

Create a bash command
```
#!/bin/zsh
mdfind -name $1 | vipe | xargs -L 1 -I {} rm -rf {}

```

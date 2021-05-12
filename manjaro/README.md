Assuming you have dvorak

```
xmodmap -pke > ~/.Xmodmap
```

then

```
xmodmap .Xmodmap
```

do it every boot

```
if [[ -f $HOME/.Xmodmap ]]; then
    xmodmap "$HOME/.Xmodmap"
fi
```
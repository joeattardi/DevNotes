Colors are defined in a colors function, source is here:
https://github.com/zsh-users/zsh/blob/master/Functions/Misc/colors

To use in a script:

```shell
autoload colors && colors
```

Then colors can be referenced by the names in the colors function. Colors are reset with `$reset_color`

```shell
$fg_bold[blue]Hello$reset_color there!
```

## Resources

- https://www.rockhoppertech.com/blog/zsh-using-color/
---
id: "WM"
aliases:
  - "Awesome"
tags:
  - "linux"
  - "window-manager"
  - "beautify"
---

# Awesome
[github](https://github.com/awesomeWM/awesome)
[config](https://github.com/worron/awesome-config)
config directory:`~/.config/awesome/`
[doc](https://awesomewm.org/apidoc/documentation/07-my-first-awesome.md.html)

[youtube](https://www.youtube.com/watch?v=JONiwmvi3q0)

## Execute commands on spawn
in the config file `rc.lua`
```lua
awful.spawn("picom --experimental-backend")
awful.spawn("polybar")
```


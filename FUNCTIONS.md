# Functions
These are extra functions you can add to your `programs.scl`. Feel free to modify them.

## TP Triggers
TP Triggers is a sub-package of Scl+, it includes Teleportation Triggers you can put on the map with specified coordinates.
Warning: These only work for triggers at the right-end side of the map.

### `tpt(location, targetX)`
```lua
function tpt(l,x) while true do if Scene.Find("hero"):position():x() => targetX then Game.EnterPortal(location,"spawn_default") end end
```
A function used to define a TP Trigger. If player passes the specified location, the player will be teleported to the specified level.

## GameShorten
GameShorten is a sub-package of Scl+, it shortens some of the Game related functions.
```lua
toast=Game.ShowNotification tp=Game.EnterPortal
```

## NTDatabase
Still in development.

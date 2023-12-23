# Scl+
Scl+ is an API for Swordigo Modders. It includes various functions and it allows you to shorten your code easily.

# How to install?
To install this package/library, head to releases and download the latest release. Find the file `programs.scl` and replace swordigo's original `programs.scl` file with the `programs.scl` you've downloaded.

# Redirects
- [Packages](./PACKAGES.md)

# Functions
## Renamed Functions
These are the functions in the original Swordigo files, but renamed to shorter names to shorten the code.
| Original Functions | Edited |
|----------|------------|
| Program.Wait | sl |
| Scene.Find | sf |
| Game.ShowNotification | t |
| Vector3.New | v3 |
| Math.RandomInt | ri |

## New Functions
These are new functions that function differently.
### `make(object, x, y)`
`make` is similar to Scene.CreateObject but it is required to give x and y for where the object should summon.
- Usage Example(s):
```lua
make("snart",5000,-182)
-- Make a snart spawn at x:5000 and y:-182.
```

### `rt(array)`
This function returns a random text from the array you provide the function with.
- Usage Example(s):
```lua
Game.ShowNotification(rt({"Hello.","Whats Up!","What ya doin?","How are you doing today?"})
-- This will print one of the options from the array.
```

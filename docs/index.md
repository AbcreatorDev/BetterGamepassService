# Documentation


<link rel="stylesheet" href="../../css/main.css">

<div class="alert">
  This is an alert box.
</div>

# Installation
## Through GitHub
1. Download the module [here](https://github.com/AbcreatorDev/BetterGamepassService/blob/main/MainModule.rbxm)
2. In Roblox Studio right click on Workspace and select 'Import from file'

![InsertModule](https://user-images.githubusercontent.com/86627085/125501504-52dce871-d3f2-4da2-9053-91c181d8b282.PNG)

3. Select the downloaded module from the 'Select a file' window

## Through Roblox

1. 'Get' the module [here](https://www.roblox.com/library/7085465779/BetterGamepassService)
2. In Roblox Studio go to the toolbox and select 'Inventory'

![GetModule](https://user-images.githubusercontent.com/86627085/125501459-292cdbd2-8b12-4c46-a7af-75539568e64f.PNG)

3. Click on the module to insert it into Workspace

# Requiring the module:

Where you would normally write the following
````Lua
game:GetService("MarketplaceService")
````
write this instead:
```Lua
require([INSERT MODULE PATH HERE])
```

### Example case:

For example if our module was located in Workspace we would write this:

```Lua
require(game.Workspace.MainModule)
```

# API Reference

## Functions

*Nothing here yet...*

## Properties

*Nothing here yet...*

## Events

*Nothing here yet...*

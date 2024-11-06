# Documentation

## Installation

### Through GitHub

1. Download the module [here](https://github.com/AbcreatorDev/BetterGamepassService/blob/main/MainModule.rbxm)
2. In Roblox Studio right click on Workspace and select 'Import from file'

  
![InsertModule](https://user-images.githubusercontent.com/86627085/125501504-52dce871-d3f2-4da2-9053-91c181d8b282.PNG)

3. Select the downloaded module from the 'Select a file' window

### Through Roblox

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

## Module

### Functions

````Lua
:SetGamePassOwnership(player : object, gamePassId : int64, wasPurchased : bool)
````
Sets the cache of the player's ownership of gamePassId to wasPurchased. This function only sets the cache for the current server, in order to have this persist a DataStore will be required.

````Lua
:PlayerHasPass(player : object, gamePassId : int64)
````
Checks if the player owns the provided gamePassId by checking through the cache / making a request (if it's not already cached)

### Properties

````Lua
.Name
````
Defaults to 'GamePassService'. **Note: Not replicated to the module script.**

````Lua
.Parent
````
Defaults to DataModel. **Note: Not replicated to the module script.**

````Lua
.Archivable
````
Defaults to true. **Note: This property is replicated to the module script.**

````Lua
.ClassName
````
Defaults to 'GamePassService'. **Note: Not replicated to the module script.**

### Events

````Lua
.OnCacheUpdated(UserId : int64, gamePassId : int64)
````
Fires when the module's custom cache is updated. The UserId field is the user id of the player that was updated in the cache and the gamePassId is the gamepass id updated in the cache.

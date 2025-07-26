# StoryTelling Mod JavaScript API Documentation

---

## API JS (api)
### `createExplosion(x, y, z)`
Creates an explosion at the specified coordinates.

### `executeCommand(command)`
Executes a Minecraft command.

### `getWorldName()`
Returns the name of the current world.

### `setBlock(blockId, x, y, z)`
Sets a block at the specified coordinates.

### `executeStory(story)`
Executes a story script, resetting all states.

### `toggleDoor(x, y, z)`
Toggles the state of a door at the specified coordinates.

---

## Automobility JS (automibility)
### `sit(npcId)`
Makes an NPC sit in the nearest automobile.

### `moveTo(npcId, x, y, z, speed)`
Moves an NPC's automobile to the specified coordinates at the given speed.

### `boost(npcId, multiplier, durationSeconds)`
Applies a speed boost to an NPC's automobile.

---

## Camera JS (camera)
### `setCamera(fromX, fromY, fromZ, toX, toY, toZ, lookX, lookY, lookZ, speed)`
Moves the camera from one position to another while looking at a target point.

### `resetCamera()`
Resets the camera to the player's original position.

### `reset()`
Resets all camera settings.

## Event Manager JS (getEvManager)
### `on(id, eventName, handler)`
Registers an event handler.

### `start(id, context, scope)`
Starts an event handler.

### `stop(id)`
Stops an event handler.

### `getHandler(id, context, scope)`
Returns a handler wrapper with start/stop methods.

---

## NPC JS (npc)
### `new npc(id, name, x, y, z, [resources])`
Creates an NPC with the specified properties.

### `getNpc(id).function();`
return npcid npc entity

### `stopAnim()`
Stops the NPC's current animation.

### `getEntity()`
Returns the NPC's entity object.

### `say(text)`
Makes the NPC say the specified text.

### `moveTo(x, y, z, speed)`
Moves the NPC to the specified coordinates.

### `teleport(x, y, z)`
Teleports the NPC to the specified coordinates.

### `playAnim(anim)`
Plays an animation on the NPC.

### `addCircleTrigger(radius, particles, callback)`
Adds a circular trigger around the NPC.

---

## Overlay JS (overlay)
### `toggle()`
Toggles the black overlay.

### `toggle(title1, title2)`
Toggles the black overlay with custom titles.

---

## Player JS (player)
### `scanForChest(x, y, z, requiredQuantity, openIfSuccess, itemId, ifPresent, ifAbsent)`
Scans a chest for items and triggers callbacks based on the result.

### `removeItemsFromChest(x, y, z, amount, itemId, ifPresent, ifAbsent)`
Removes items from a chest and triggers callbacks.

### `scanForBlock(centerX, centerY, centerZ, radius, blockId, ifPresent, ifAbsent)`
Scans for a block in a radius and triggers callbacks.

### `getItemPlayer(itemId, ifPresent, ifAbsent)`
Checks if the player is holding an item and triggers callbacks.

### `hasItemInInventory(itemId, ifPresent, ifAbsent)`
Checks if the player has an item in their inventory and triggers callbacks.

### `say(text)`
Makes the player say the specified text.

### `giveItem(itemId)`
Gives the player an item.

### `getX()`, `getY()`, `getZ()`
Returns the player's coordinates.

---

## Quest JS (qyest)
### `getState(id)`
Returns the state of a quest.

### `addQuest(id, title, description, reward, fail)`
Adds a new quest.

### `acceptQuest(id)`
Accepts a quest.

### `completeQuest(id)`
Completes a quest.

### `failQuest(id)`
Fails a quest.

### `clear()`
Clears all quests.

---

## Scene JS (scene)
### `time(() => { runnable },[int])`
Schedules a callback to run after a delay.

### `reset()`
Resets all scene actions and tasks.

---

## Screen JS (player)
### `new Screen(id, question, restArray)`
Creates a dialog screen with options.

### `show(getNpc(id).getEntity())`
Shows the dialog screen to the specified entity or player.

### `show()`
Shows the dialog screen

### `getScreen(id, context, scope)`
Returns a screen wrapper for the specified ID.
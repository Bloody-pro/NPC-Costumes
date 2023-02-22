
<p align="center">
  <img src="https://user-images.githubusercontent.com/77890259/220716849-8b19b8d3-58aa-4e22-a73c-ca5d2c02d8a5.png?raw=true" alt="Sublime's custom image" width="50%" height="50%"/>
</p>

## *A plugin to easily create Slapper-esque NPCs with custom geometry which can trigger set commands on right and left clicks along with collisions.*

# SETUP EXAMPLE + CONFIG SPOONFEEDING
Go to the skins.yml and add an indented section under 'skins:' and give it a name. In this example, I called it kitnpc. Write down the display name of your skin after 'displayname'. (This is NOT the display name of the actual NPC!) This is the name provided in the skin selector that only you can see. Write the file name of your 64x64 texture beside 'texture:'. In this example, it is called kitNPC.png. Do the same for your .json model file. Finally, add your model identifier next to 'identifier:'. If you're wondering what the hell an identifier is, it's in your .json file.

*kitNPC.json*
```
{
	"format_version": "1.12.0",
	"minecraft:geometry": [
		{
			"description": {
				"identifier": "geometry.kitnpc",
        ...
```
*skins.yml*
```
skins:
  kitnpc:
    displayname: 'KitNPC' 
    texture: 'kitNPC.png'
    json: 'kitNPC.json' 
    identifier: 'geometry.kitnpc' 
```

### INGAME SETUP
Run the command /npc. This will pull up a form.


###### Concept suggested by '! VrisQ#0700' on the PocketMine-MP discord.

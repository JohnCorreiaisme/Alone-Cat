# Alone Cat

You play as Biscuits, a fat, fluffy, very hungry house cat. The human has been locked up for three days, the food bowl is empty, and nobody is coming. Get out of the apartment and find your way home: down the alley, through the sewer maze of the Raccoon King, and across a junkyard where a skunk wants his throne back.

It's a kid-friendly 3D browser game built with [three.js](https://threejs.org/) (r128). Nothing dies; animals that lose a fight just run away.

## Play

Open `index.html` through a local web server. Opening the file directly won't load the models and sounds, because browsers block file access from `file://` pages.

```bash
python -m http.server 8000
```

Then visit <http://localhost:8000>.

On the title screen you can choose **3D models** (the default) or **Classic sprites**, the original painted sprite look. Your choice is remembered.

## Controls

| Keyboard / mouse | Controller | Action |
|---|---|---|
| W A S D / arrows | Left stick / D-pad | Move |
| Drag the mouse | Right stick | Turn the camera |
| Space | A | Jump and climb |
| E | X or B | Swipe or use (swipes if something is in range, otherwise interacts) |
| Q | Y | Meow |
| Shift | RT or click the left stick | Sprint |
| Ctrl / C | LT | Stalk |
| Esc / P | Start | Pause |
| M | Back | Mute |

Your **Tummy** drains all the time. When it's empty it eats your lives instead, so eat everything.

## Levels

1. **The Apartment**: escape the bedroom and find a way out of the flat.
2. **The Alley**: get down the fire escape and past the strays.
3. **The Sewers**: a maze with the Raccoon King at its heart.
4. **The Junkyard**: help the Skunk King take his throne back from his brother, the Baron.

## Files

- `index.html`: the whole game.
- `*.png`, `*.jpg`: sprite sheets, props and textures.
- `*_model.json` + `*_model_tex.jpg`: rigged, animated 3D models (glTF stored as JSON) for Biscuits, strays, dogs, raccoons and skunks.
- `intro.mp4`: the opening clip.
- `snd/`: cat sounds.

## Credits

- Cat sounds: CC0 recordings from [BigSoundBank](https://bigsoundbank.com/). All other sounds are generated in the browser.
- 3D models were made from the game's own sprite turnarounds, using Hunyuan3D in ComfyUI, then painted and rigged in Blender.

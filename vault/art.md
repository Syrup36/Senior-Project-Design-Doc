---
id: HTAUxWlHBnNkYOOiCN6Eo
title: Art
desc: ''
updated: 1644851724345
created: 1643737944911
---
*last updated {{fm.updated}}*

## Tools
All 3D models will be create in [Blender](https://www.blender.org/), while all 2D assets will be created either in [Inkscape](https://inkscape.org/), [GIMP 2](https://www.gimp.org/), or [Aseprite](https://www.aseprite.org/).

## Style
The game will be in a **low-poly style**. I have the most experience creating and rigging low-poly models, so this choice should streamline asset creation. Using a more simple style will also allow assets to be much smaller in size, demand less rendering resources, and will thus make the game able to be run on a wide variety of devices.

To make development easier, the UI will follow a more minimal design. This makes it easier to go from a UI prototype to the final product, as new assets generally won't have to be created.

Colors will stick to a specific color palette:

>TODO: ADD COLOR PALETTE HERE

>TODO: Insert Images of 3D Models Here

## Post Processing
Post processing will be applied as needed. I don't know much about color grading, but I assume some of it will be necessary.

## Animations
Since I don't have much experience with animating objects (but still feel confident in my abilities), the game will have a few animations:
- Walking/Running
- Idle
- Falling
- Talking Gestures

Characters facial expressions will either be additional textures or seperate models.

>Below is sample code that I create on the spot and wanted to write down for the future. Please ignore it.

```CS
void OnDialogueDisplay() 
{
    if(transform.children[0].name == dialogueObject.requiredExpression)
    {
        //Replace Facial Expression
    }
    return;
    //Don't replace transform/texture if expression remains the same, to save on resources.
}
```

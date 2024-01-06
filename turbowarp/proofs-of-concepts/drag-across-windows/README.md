# Drag Across Windows

`v2.0.0`

With TurboWarp and a bit of magic, I managed to break the boundaries of the project and transfer draggable items from one window to another, without even using Cloud variables like you might have expected with this sort of feature.

## How to use it

Click an item to pick it up and click it again to place it. To transfer an item to another window, simply open two or more instances of the same project and drag the item outside the confines of one project player and into another.

## How it works

When you pick up an item and move it outside the stage borders, the project writes information about the dragged item to local storage, which can then be read by other instances of the project. This essentially allows the project to transfer data to other instances of itself. In this case, it is transferring data about the item you're dragging.

The built-in demo for this proof of concept transfers three properties, one number for the costume and two coordinates representing the item's offset from the mouse pointer, but you can add more properties to transfer by changing the code.

When you place the item after dragging it across windows, the item in storage is cleared to communicate with every window that the item was placed and to stop dragging it.

As I said earlier, the project does not use Cloud variables, so it works offline but you can only drag between windows on the same device.

## Using it in your projects

This is mostly a proof of concept to show that this is possible and to try something new, but you may use this tool in your projects! Here's a few tips:

- **I have organized the code in the one included sprite such that anything off to the right is necessary for Drag Across Windows to function (be careful modifying it, otherwise you might break something, but you can and should look at it so that you can learn how it works) and anything on the left can be modified as you wish.**
- Everything is self-contained in the one included sprite, so all you have to do is import that one thing and you're off!
- You have to click twice, once to pick up and once to place. The reason I went with this behavior is because, in Windows at least, if you hold down the mouse button while moving the cursor outside the window, only that window will be able to tell where your mouse is going and that your mouse button is down, until you release it.
- If the clones acting as the draggable items are running code, then the code will be restarted when the item is placed. This happens because when you pick up the item, the clone is actually deleted and the parent sprite takes on its appearance, then a new clone is created when you place it.

## Credits and license

Thanks to the following [TurboWarp extensions](https://extensions.turbowarp.org/) for making this possible:
- [Local Storage](https://extensions.turbowarp.org/local-storage.js)
- Skyhigh173's [JSON](https://extensions.turbowarp.org/Skyhigh173/json.js)

I also used the [Runtime Options](https://extensions.turbowarp.org/runtime-options.js) extension to make the project compatible with any stage size.

The shape tiles come from my project [Shape Board Pro](https://scratch.mit.edu/projects/798778469/) on Scratch, which is under a CC-BY-SA 2.0 license; (Ͻ) 2023 D-ScratchNinja.

Drag Across Windows as a whole is licensed under the terms of CC-BY-SA 2.0, (Ͻ) 2024 DNin01 from GitHub. The code is licensed separately, under the terms of CC-BY 4.0, (Ͻ) 2024 DNin01 from GitHub.

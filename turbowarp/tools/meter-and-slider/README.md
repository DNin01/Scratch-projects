## Meter and Slider Documentation

`v0.1.0`

### Overview

This project gives you a lightweight setup to easily make horizontal meters (for example, progress bars) that look like almost whatever you want and have no drawbacks such as requiring a bunch of costumes or the Pen extension, except for a hopefully easily resolvable visual issue. It also lets you add a visual-only slider handle with one setting!

**Open this project in [TurboWarp](https://turbowarp.org/).**

### How to use

#### The basics

The included sprite comes with everything you'll need to get started. The following custom block is where the magic happens:
```
place meter (n) full at x: (x) y: (y) width: (w) slider? <slider>
```

Just fill in the following:
| Argument | Description |
|:---:|:---:|
| _n_ | A number from 0 to 1 indicating how close to full the meter will be |
| _x_ and _y_ | The x and y coordinates of where you want your meter to be placed |
| _w_ | The width of the meter costumes |
| _slider_ | Whether you want the meter to have a slider handle |

Or start by loading up the project and playing around. You'll get it right away.

#### Customizing the looks

To change the design of the meter, just go into the costume editor and modify the three costumes to your liking. If you change the width of the first two costumes in the process, be sure to plug the new width value into uses of the custom block.

### Other

Note:
- You might notice the meter break up sometimes, due to the way it's rendered (in Scratch, visuals are never perfect). You might be able to quickly resolve this by modifying one of the "set clipping box" blocks under the custom block definition, or, even easier, just removing the first "set clipping box" block entirely.
- The slider handle is not pre-programmed to be adjustable by dragging. Technically, you could modify it to make it adjustable, though!

This project uses [Vadik1](https://scratch.mit.edu/users/Vadik1/)'s [Clipping & Blending](https://extensions.turbowarp.org/Xeltalliv/clippingblending.js) TurboWarp extension.

---

(Ͻ) 2023 DNin01 from GitHub. Available under a CC-BY-SA 2.0 license.

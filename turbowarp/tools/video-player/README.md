## Video Player Maker

`v0.5.0`

This project gives you the basic components for making videos and animations that users can fast-forward, rewind, and pause.

> [!NOTE]
> This video player does not come with audio track seeking support... yet.

It's possible to control the video by using the controls at the bottom of the player or with keyboard shortcuts.

### How to use

#### Getting set up

The "Progress bar" sprite contains all the essential components to make the video player run. The "Flower" sprite is just a demo animation that you can use as a reference. You can take just "Progress bar" if you're making something.

#### Setting the scene

Set the variable "Duration" to the length of your video in frames.

> [!TIP]
> Scratch runs at 30 frames per second, so the duration is measured in 1/30ths of a second.

One of the default scripts sets this value to 1,800 (which equals 60 seconds), so modify that value to change the duration.

This project works the same at any framerate, by calculating the speed at which it would run if it were still at 30 FPS, so if you're going to change the framerate, just refer to a "frame" as 1/30th of a second.

From there, just create your video's code! Use the "Time" variable to get the current time of the video in frames.

> [!NOTE]
> If you change the framerate, this might be a decimal number.

That's about it!

### Credits

Thanks to the following [TurboWarp extensions](https://extensions.turbowarp.org/) for making this possible:
- [Mouse Cursor](https://extensions.turbowarp.org/cursor.js)
- Scratch Lab's [Animated Text](https://extensions.turbowarp.org/lab/text.js)
- JeremyGamer13's [Tweening](https://extensions.turbowarp.org/JeremyGamer13/tween.js)
- TrueFantom's [Couplers](https://extensions.turbowarp.org/true-fantom/couplers.js)

I also used the [Runtime Options](https://extensions.turbowarp.org/runtime-options.js) extension to make the project work at any framerate.

---

(Ͻ) 2023 DNin01 from GitHub. Available under a CC-BY-SA 2.0 license.

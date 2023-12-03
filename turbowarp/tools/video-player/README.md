## Video Player Maker

`v0.6.0`

This project gives you the basic components for making videos and animations that users can fast-forward, rewind, and pause, in addition to an already-functional UI.

> [!NOTE]
> This video player does not come with audio track seeking support... yet.

It's possible to control the video by using the controls at the bottom of the player or with keyboard shortcuts.

### How to use

#### Getting set up

The "Progress bar" sprite contains all the essential components to make the video player run. The "Flower" sprite is just a demo animation that you can use as a reference. You can take just "Progress bar" if you're making something.

#### Setting the scene

To get started, we'll need to configure the video. There are two important configuration variables.

First is `MEASUREMENT_UNIT`. Video Player Maker allows you to set the unit of measurement used by your video's code. This could be seconds, frames, milliseconds, anything. It determines how many seconds it takes for the `Time` variable to go up by 1, so if this variable is set to `2`, then `Time` equals the current number of seconds divided by 2. If you want to measure in fractions of a second, you can insert a division operator to set a more precise value.

Your code can then access the video's current time measured as you configured it via the `Time` variable.

Second is `DURATION_FRAMES`. It should be set to the length of your video in 1/30ths of a second. Why 1/30ths of a second? Well, Scratch runs at 30 frames per second, so Video Player Maker measures the duration internally in that unit of time.

You probably know that TurboWarp lets you change the framerate and might be wondering what that means for your videos. While the project often uses the term "frame", your video will not speed up or slow down based on the framerate because Video Player Maker makes some calculations to ensure the video always runs at the same speed as it would at 30 FPS. In fact, the demo project runs at 60 FPS by default.

If you're going to change the framerate, just refer to a "frame" (as a measurement unit) as 1/30th of a second.

#### Setting up your video's content

To start making a video, you just need to code it. Use the `Time` variable as mentioned before to get the current time (measured in `MEASUREMENT_UNIT` seconds).

> [!IMPORTANT]
> 1. Note that the value of the `Time` variable can be a decimal and may skip a beat when delta time is being used, so don't rely on `=` or even `round` operations with it. Instead, check when it surpasses a timestamp (a "not less than" operation would be the best) if you want to trigger an event at a certain time.
>
> 2. You'll probably want to layer your video's content below the "Progress bar" sprite. You can do this by running `go to (back v) layer` on the sprites belonging to your video, or by running `go to (front v) layer` on the "Progress bar" sprite. This also helps with code execution order (if you notice some lag and you've layered the sprites correctly, try clicking the green flag on the project player again).

In case you ask, yes, you can safely initialize and even run a loop to update the sprites in your video on green flag.

You can update the sprites in your video every frame with no problem, but you can also refresh them whenever a `refresh screen` message is broadcasted, by using a `when I receive (refresh screen v)` hat block. This message is sent by Video Player Maker while the video is playing or being scrubbed, so it's basically a signal to render content. The advantage of this is that your code won't have to run when the video is paused.

Keep in mind that the user can pause and scrub to any point in the video at any time.

That's about it!

### Credits

Thanks to the following [TurboWarp extensions](https://extensions.turbowarp.org/) for making this possible:
- [Mouse Cursor](https://extensions.turbowarp.org/cursor.js)
- My [Wake Lock](https://extensions.turbowarp.org/DNin/wake-lock.js)
- Scratch Lab's [Animated Text](https://extensions.turbowarp.org/lab/text.js)
- [Runtime Options](https://extensions.turbowarp.org/runtime-options.js)
- XeroName's [Deltatime](https://extensions.turbowarp.org/XeroName/Deltatime.js)
- JeremyGamer13's [Tweening](https://extensions.turbowarp.org/JeremyGamer13/tween.js)
- TrueFantom's [Couplers](https://extensions.turbowarp.org/true-fantom/couplers.js)

---

(Ͻ) 2023 DNin01 from GitHub. Available under a CC-BY-SA 2.0 license.

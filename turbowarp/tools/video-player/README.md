## Video Player Maker Documentation

v0.1.0

### Overview

This project gives you the basic components for making videos and animations that users can fast-forward, rewind, and pause.

This project can be opened in [TurboWarp](https://turbowarp.org/).

### How to use

The "Progress bar" sprite contains all the essential components to make the video player run. The "Flower" sprite is just an example animation that you can use as a starter. Take both of them with you to start, or just "Progress bar" if you're brave or you know how it works.

Set the variable "Duration" to the length of your video in 1/30ths of a second. The main-loop script sets it to 1,800 (which means 60 seconds) by default, so modify that value to change the duration.

This project is compatible with any frame rate. It uses the "get framerate" block from the Runtime Options TurboWarp extenstion to calculate delta time.

That's about it!

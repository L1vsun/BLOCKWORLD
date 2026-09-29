# Build log

The real session log, written by the model as it worked. All times are local, 2026-09-29.

```
2026-09-29 20:15:57  log opened, owner away (task: build a playable voxel sandbox game in the browser)
2026-09-29 20:18:47  game.js started
2026-09-29 20:27:24  first full render: terrain, biomes, caves, trees, water, sky, lamps
2026-09-29 20:31:06  fix: black fringes on leaves/grass (canvas premultiplied alpha -> raw DataTexture atlas)
2026-09-29 20:31:06  fix: plants lit from below on back faces (both windings, up normal)
2026-09-29 20:31:06  playtest passed: spawn, walk, jump, fly, raycast break + place
20:31-20:37          lighting tuned for the video: water specular colour, moonlight, ambient (3 constants)
2026-09-29 20:37:49  video capture of the game started
2026-09-29 20:59:01  packaged as this repo: index.html, README, licenses, screenshots
2026-09-29 21:05:48  laptop pass: graphics presets (G), adaptive resolution, trackpad/Mac input, battery throttle; tested in Chromium + WebKit
2026-09-29 21:14:40  fix: "click to play" did nothing (lock listener was on the canvas, under the overlay); now on the document + a hint if the browser refuses
```

The two fixes at 20:31 were found by the model while checking its own renders. Nobody reported
them.

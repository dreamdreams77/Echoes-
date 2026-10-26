# Optional art assets

The game draws all of its art in code, so this folder can stay empty. To override any piece with your own images (for example ones made with an AI image generator), put the files here and list them in `manifest.json`:

```json
{ "sky": "sky.webp", "title": "title.webp", "ground": "ground.webp", "brick": "brick.webp" }
```

| Key | What it is | Suggested size | Notes |
|-----|-----------|----------------|-------|
| `sky` | 360-degree sky, equirectangular, 2:1 | 2048x1024 | Left and right edges should match. Keep the bottom half dark or plain; it is hidden by terrain. |
| `title` | Title screen backdrop | 1920x1080 | Dark in the middle so the text stays readable. |
| `ground` | Seamless grass or dirt texture | 512x512 | Mid grey tones; it is tinted by the terrain colours. |
| `brick` | Seamless stone brick texture | 512x512 | Mid grey tones; it is tinted per wall. |

Use WebP or JPEG and keep each file under about 500 KB.

Example prompts:
- sky: "painted fantasy dusk sky, soft violet and amber clouds, wide panorama, no ground, no sun disc"
- ground: "seamless tileable mossy grass ground texture, top-down, muted green, hand painted"
- brick: "seamless tileable weathered grey castle stone bricks texture, front view"

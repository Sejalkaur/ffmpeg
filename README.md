Commands used:
### Chnaged resolution And did compression

```bash
ffmpeg -i input.mp4 -c:v libx264 -crf 28 -preset medium -c:a aac -b:a 128k output_compressed.mp4
```
### Add Logo to the video
```bash
ffmpeg -i input.mp4 -i logo.avif -filter_complex "overlay=W-w-20:20" -c:v libx264 -crf 23 -preset medium -c:a copy output_with_logo.mp4
```

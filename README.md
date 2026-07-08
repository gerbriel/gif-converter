# gif-converter

High-quality MP4 → GIF conversion that runs entirely in your browser.

**Live site:** https://gerbriel.github.io/gif-converter/

## How it works

- Drop in any video your browser can play (MP4, MOV, WebM…)
- Frames are decoded locally with a `<video>` element and a canvas — **nothing is uploaded**
- Each frame is quantized to its **own 256-color palette** (the same trick [gifski](https://gif.ski) uses), which keeps on-screen text and gradients crisp instead of muddy
- Encoding by [gifenc](https://github.com/mattdesl/gifenc) (MIT), vendored in `gifenc.esm.js`

## Options

| Option | Notes |
| --- | --- |
| Frame rate | 10–24 fps; higher = smoother and larger |
| Size | Keep **Original** when the video contains text |

## Also in this repo

`Gifski/` contains the source of the excellent native macOS app [sindresorhus/Gifski](https://github.com/sindresorhus/Gifski) (MIT), kept here for reference. For desktop conversion, that app is the gold standard.

# ASTC Texture Decoder

A professional-grade, browser-based tool for decoding [ASTC (Adaptive Scalable Texture Compression)](https://en.wikipedia.org/wiki/Adaptive_Scalable_Texture_Compression) files. This project uses WebAssembly for high-performance decoding and supports batch processing.

This tool allows you to:
* **Batch Upload:** Upload multiple `.astc` files from your device.
* **Load from URL:** Load individual `.astc` files from a web URL.
* **Cumulative Decoding:** Decode multiple batches; new results are added to the page without clearing previous ones.
* **Instant Preview:** Preview each decoded image on its own canvas.
* **Flexible Downloads:**
    * **Download PNG(s):** Download one or more images as individual `.png` files.
    * **Download All as ZIP:** Download multiple images (2 or more) as a single, convenient `.zip` file.
* **Clear Control:** Manually clear all results with a dedicated "Clear Results" button.

## What is ASTC?
ASTC is an advanced texture compression format used primarily in mobile and web graphics, offering excellent quality at various compression ratios.

## Decoding ASTC in the Web
Decoding ASTC in the browser requires a custom decoder. This project uses a C++ decoder compiled to **WebAssembly (WASM)**, which allows it to run at near-native speed. The JavaScript code acts as an interface to:
1.  Load the `.astc` file data.
2.  Pass the data to the WASM decoder.
3.  Receive the raw RGBA pixel buffer.
4.  Display the result on an HTML `<canvas>`.

## Resources
- [ARM-software/astc-encoder (Official Reference)](https://github.com/ARM-software/astc-encoder)
- [Basis Universal WASM Decoder](https://github.com/BinomialLLC/basis_universal)

---

**Made by KingofGames**
- **Telegram:** [t.me/KingofGames02](https://t.me/KingofGames02)

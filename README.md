# ASTC Texture Decoder

A professional-grade, browser-based tool for decoding [ASTC (Adaptive Scalable Texture Compression)](https://en.wikipedia.org/wiki/Adaptive_Scalable_Texture_Compression) files. This project uses WebAssembly for high-performance decoding and supports batch uploading.

This tool allows you to:
* Upload multiple `.astc` files at once.
* Decode them instantly in the browser.
* Preview each decoded image on its own canvas.
* Download all decoded images as a single `.zip` file.

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

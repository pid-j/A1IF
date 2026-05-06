# A1IF image format

<img width="240" height="160" alt="A1IFLogo" src="https://github.com/user-attachments/assets/7074dd99-0b9e-49c8-b1cf-fc1b13fe1d4f" />

## 1. Introduction
A1IF, which stands for Abstracted 1-Bit Image Format, is an image format designed to have two colors - black and white. Unlike a raw 1 bit image, it doesn't store one bit at a time; rather, it starts with the black state at the left edge of the screen. Whenever it encounters a white color, it flips and records that for the line. The color then flips and it does the same for a black color, and vice versa. This is why the name has "Abstracted" because it doesn't store the pixels, but instead stores the flips between rows of colors.

## 2. Features
This sprite has a full scanner and drawer, allowing for easy use. A demo script is provided, and you can use the green flag and then press the space key or click to scan the provided image. To change the image, use the right and left arrow keys. You can also make your own image but it has to be transparent; using a solid background won't work.

## 3. Comparisons 
For the provided images in the Scan sprite:

- Image 1 - black
- .PNG export: 13.2KB
- A1IF scan: 1.4KB (~90% filesize decrease!!!)

---

- Image 2 - badapple
- .PNG export: 21.1KB
- A1IF scan: 3.6KB (~82% filesize decrease!)

---

- Image 3 - Male_and_female_chicken_sitting_together
- .PNG export: 69.1KB
- A1IF scan: 35.3KB (~41% filesize decrease!)

---

- Image 4 - ilikebirds
- .PNG export: 51.9KB
- A1IF scan: 7.1KB (~86% filesize decrease!)

As you can see, the A1IF scans tend to have a smaller filesize by an average of 80%. This makes sense due to the fact that PNGs don't just store white and black, they store other colors too. There's probably some other technical reason too, but I don't know. I don't know how the comparison to JPEG is, but I don't really care. What's important is this doesn't use binary so you can be assured that there will be no corruption, even on non-TW projects!

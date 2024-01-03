# Valence Brand Guide
1. **[Overview](#)**
2. **[Identity Elements](#)** / [Blurred Red Circle](#), [Black Circle](#), [18 Moons](#), [The Diagram](#), [Wordmark](#)
3. **[In Use](#)** / [The Diagram Only](#), [Wordmark Only](#), [Lockups](#)
4. **[Colors](#)** / [Brand Colors](#), [Graphing Colors](#)
5. **[Typography](#)** / [Primary Typeface](#), [Secondary Typeface](#), [Tertiary Typeface](#)
6. **[Sample Designs](#)**
7. **[Contact](#)**

## 1. Overview
TKTK

## 2. Identity Elements
Valence brand's visual identity consists [Blurred Red Circle](#a-blurred-red-circle), [Black Circle](#b-black-circle), and [18 Moons](#c-18-moons), that make up [The Diagram](#d-the-diagram). It can be used in conjunction with the [wordmark](#e-wordmark).

![Identity Elements](https://placehold.co/1920x1080)

### a. Blurred Red Circle

The red circle's blur can be reproduced in Figma with [Layer Blur](https://help.figma.com/hc/en-us/articles/360041488473-Apply-shadow-or-blur-effects#blur), with the amount to be set as 12.5% of the diameter. In SVG or CSS, the amount should be set as 6.25%.

| Diameter | Figma Layer Blur `12.5%` | SVG feGaussianBlur `6.25%` | CSS Blur `6.25%` |
| -------- | ------------------------ | -------------------------- | ---------------- |
| 400px    | 50                       | 25                         | 25               |

Example in SVG:
```
<svg width="500" height="500" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
  <circle cx="250" cy="250" r="200" fill="#FF2B00" filter="url(#blur)" />
  <filter id="blur" x="0" y="0" width="500" height="500" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
    <feGaussianBlur stdDeviation="25"/>
  </filter>
</svg>
```
Example in HTML/CSS:
```
<div class="blurred-red-circle"></div>
<style>
  .blurred-red-circle {
    width: 400px;
    height: 400px;
    background: #FF2B00;
    border-radius: 200px;
    filter: blur(25px);
}
</style>
```

### b. Black Circle

Black Circle should always appear in the same diameter (without blur) as the Blurred Red Circle. 

### c. 18 Moons

![18 Moons Configuration](https://placehold.co/1920x1080)

Each moon is drawn on the same diameter circular path, 20 degrees apart from each other. Each moon's diameter is 6.25% of the primary diamter.

### d. The Diagram

The diagram is where the three identity elements overlap. Blurred Red Circle and Black Circle are positioned on top of another with 50% of their height overlapping. The overlapped area is represented in blue, [the opposite end of the specific red in HSL color space](#a-brand-colors). 18 moons are placed at the center of the composition with each moon colored as an opposite of its surrounding.

![The Diagram Configuration](https://placehold.co/1920x1080)

### e. Wordmark

Valence wordmark is a customized rendition of [Times](#a-primary), the primary typeface of the brand.

![Wordmark Configuarion](https://placehold.co/1920x1080)

## 3. In Use

### a. The Diagram only

The diagram can be used by itself to represent the Valence brand where approproate.

![The Diagram only](https://placehold.co/1920x1080)
Download [SVG](#), [PNG](#)

### b. Wordmark only

The wordmark can be used by itself to represent the Valence brand where approproate.

![Wordmark only](https://placehold.co/1920x1080)
Download [SVG](#), [PNG](#)

### c. Lockups

The Diagram and Wormark can be locked up in two different ways. Horizontal lockup is preferred when there's limites surface amount to utilize. Vertical lockup is preferred for more official use.

![Horizontal lockup](https://placehold.co/1920x1080)
Download [SVG](#), [PNG](#)

![Vertical lockup](https://placehold.co/1920x1080)
Download [SVG](#), [PNG](#)

## 4. Colors
### a. Brand colors

![HSL Color Space](https://placehold.co/1920x1080)

![Brand colors](https://placehold.co/1920x1080)

The primary colors for Valence are listed below. These are the same colors used in the Blurred Red Circle, Black Circle and and the overlapped area.

|                                                   | Name   | HSL             | RGB             | HEX       |
| ------------------------------------------------- | ------ | --------------- | --------------- | --------- |
| ![](https://placehold.co/15x15/FF2A00/FF2A00.png) | Red    | ` 10, 100,  50` | `255,  42,   0` | `#FF2A00` |
| ![](https://placehold.co/15x15/000000/000000.png) | Black  | `  0,   0,   0` | `  0,   0,   0` | `#000000` |
| ![](https://placehold.co/15x15/02D5FF/02D5FF.png) | Blue   | `190, 100,  50` | `  2, 213, 255` | `#02D5FF` |


### b. Graphing colors

A separate set of colors, primarily to differentiate different categories shwon in charts and graphs, is defined as below. These colors are chosen with perceptually distinction and verbal describability in mind. 

The color set is also designed to be used in order. If you want only four colors, the first four colors from the list can be used, as the colors at the top of the list are more identifiable. It is best practice to keep the number of colors to a minimum in a single chart.

Please note that while the red is the same red as the brand color, but the blue is different for better legibility.

```
'#FF2A00' ,'#00A3FF' ,'#EA80D1' ,'#4EBB5B' ,'#FFBC57' ,'#800000' ,'#A0A0A0' ,'#C2C600' ,'#8476DE' ,'#17CFCF'
```

|                                                   | Name   | HSL             | RGB             | HEX       |
| ------------------------------------------------- | ------ | --------------- | --------------- | --------- |
| ![](https://placehold.co/15x15/FF2A00/FF2A00.png) | Red    | ` 10, 100,  50` | `255,  42,   0` | `#FF2A00` |
| ![](https://placehold.co/15x15/00A3FF/00A3FF.png) | Blue   | `202, 100,  50` | `  0, 163,  55` | `#00A3FF` |
| ![](https://placehold.co/15x15/EA80D1/EA80D1.png) | Pink   | `314,  71,  71` | `234, 128, 209` | `#EA80D1` |
| ![](https://placehold.co/15x15/4EBB5B/4EBB5B.png) | Green  | `127,  44,  52` | ` 87, 187,  91` | `#4EBB5B` |
| ![](https://placehold.co/15x15/FFBC57/FFBC57.png) | Yellow | ` 36, 100,  62` | `255, 177,  60` | `#FFBC57` |
| ![](https://placehold.co/15x15/800000/800000.png) | Brown  | `  0, 100,  25` | `128,   0,   0` | `#800000` |
| ![](https://placehold.co/15x15/A0A0A0/A0A0A0.png) | Gray   | `  0,   0,  63` | `160, 160, 160` | `#A0A0A0` |
| ![](https://placehold.co/15x15/C2C600/C2C600.png) | Olive  | ` 61, 100,  39` | `194, 198,   0` | `#C2C600` |
| ![](https://placehold.co/15x15/8476DE/8476DE.png) | Purple | `248,  61,  67` | `132, 118, 222` | `#8476DE` |
| ![](https://placehold.co/15x15/17CFCF/17CFCF.png) | Teal   | `180,  80,  45` | ` 23, 207, 207` | `#17CFCF` |

These are good to be used on a white, black or a light gray background as accent.

|                                                   | Name         | HSL             | RGB             | HEX       |
| ------------------------------------------------- | ------------ | --------------- | --------------- | --------- |
| ![](https://placehold.co/15x15/FFFFFF/FFFFFF.png) | White        | ` 10, 100,  50` | `255, 255, 255` | `#FFFFFF` |
| ![](https://placehold.co/15x15/000000/000000.png) | Black        | `202, 100,  50` | `  0,   0,   0` | `#000000` |
| ![](https://placehold.co/15x15/E9E9E9/E9E9E9.png) | Light gray   | `  0,   0,  91` | `233, 233, 233` | `#E9E9E9` |

## 5. Typography
### a. Primary typeface

The primary typeface for Valence brand is Times, a classic typeface with rich history. There are many digital variants of Times typeface, including Times (Linotype) included in macOS, and Times New Roman (Monotype) in Windows. While they are very similar and therefore interchangeable, the brand prefers Times (Linotype), the digitalized version of the typefaced commissioned by the newspaper The Times.

The typeface can be used for brand messages and body text. However, for UI use, Times can be replaced with a font that has a slightly refined look, including Adobe Text Pro.

![Primary typeface](https://placehold.co/1920x1080)

### b. Secondary typeface

The secondary typeface, to be used in conjunction with the primary, is Unica 77 by Lineto. Unica 77 is versatile enough to be used in UI applications. The license for Unica 77 can be obtained from [Lineto website](https://lineto.com/typefaces/unica77?font=L3l-qxAYPaV).

![Primary typeface](https://placehold.co/1920x1080)

### c. Tertiary typeface

For a limited use, for visual clarity in numeric and code representation, the [monospaced variant of Unica 77](https://lineto.com/typefaces/unica77-mono?font=PDpITQJkbYI) can be used. Proper licenses to be obtained upon usage.

![Primary typeface](https://placehold.co/1920x1080)

## 6. Sample designs



## 7. Contact
For inquiries, please contact TKTK.
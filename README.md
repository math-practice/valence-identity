# Valence Brand Guide
1. **[Overview](#1-overview)**
2. **[Identity Elements](#2-identity-elements)** / [Blurred Red Circle](#a-blurred-red-circle), [Black Circle](#b-black-circle), [18 Moons](#c-18-moons), [The Diagram](#d-the-diagram), [Wordmark](#e-wordmark)
3. **[In Use](#3-in-use)** / [The Diagram Only](#a-the-diagram-only), [Wordmark Only](#b-wordmark-only), [Lockups](#c-lockups)
4. **[Colors](#4-colors)** / [Brand Colors](#a-brand-colors), [Graphing Colors](#b-graphing-colors)
5. **[Typography](#5-typography)** / [Primary Typeface](#a-primary-typeface), [Secondary Typeface](#b-secondary-typeface), [Tertiary Typeface](#c-tertiary-typeface)
6. **[Sample Designs](#6-sample-designs)**
7. **[Contact](#7-contact)**

## 1. Overview
TKTK

## 2. Identity Elements
Valence brand's visual identity consists of three same size circles – [blurred red circle](#a-blurred-red-circle), [black circle](#b-black-circle), and [18 Moons](#c-18-moons). These circles make up [the diagram](#d-the-diagram), which can be used in conjunction with the [wordmark](#e-wordmark). Refer to [lockups](#c-lockups) section for detail.

![Identity Elements](images/identity-elements.svg)

### a. Blurred Red Circle

The blurred red circle is can be reproduced in Figma with [Layer Blur](https://help.figma.com/hc/en-us/articles/360041488473-Apply-shadow-or-blur-effects#blur) function, with the amount to be set as 12.5% of the diameter. In SVG or CSS, the amount should be set as 6.25%. Below is an example when the circle is 400px in diameter:

| Diameter | Figma Layer Blur `12.5%` | SVG feGaussianBlur `6.25%` | CSS Blur `6.25%` |
| -------- | ------------------------ | -------------------------- | ---------------- |
| 400px    | 50                       | 25                         | 25               |

The blurred red circle in SVG:
```html
<svg width="500" height="500" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
  <circle cx="250" cy="250" r="200" fill="#FF2B00" filter="url(#blur)" />
  <filter id="blur" x="0" y="0" width="500" height="500" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
    <feGaussianBlur stdDeviation="25"/>
  </filter>
</svg>
```
The blurred red circle in HTML/CSS:
```html
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

The black circle should always appear in the same diameter (without blur) as the blurred red circle, in pure black.

### c. 18 Moons

The third circle consists of 18 dots. Each dot (moon) is drawn on the circular path of the same diameter as otehr circles, 20 degrees apart from each other. Each moon is 6.25% in size of the primary circle.

![18 Moons Configuration](images/18-moons-configuration.svg)

### d. The Diagram

The diagram is where the three identity elements overlap, which can be used as standalone element. See [In Use](#3-in-use) section for further detail. The blurred red circle and the black circle are positioned on top of another with 50% of their height overlapping. The overlapped area is represented in blue, [the opposite end of the specific red in HSL color space](#a-brand-colors). 18 moons are placed at the center of the composition with each moon colored as an opposite of its surrounding.

![The Diagram Configuration](images/the-diagram-configuration.svg)

### e. Wordmark

Valence wordmark is a customized rendition of [Times](#a-primary), the primary typeface of the brand. Below is a diff of the Valence wordmark and the word 'Valence' set in Times. The wordmark can be used as standalone element. See [In Use](#3-in-use) section for further detail.

![Wordmark Configuration](images/wordmark-configuration.svg)

## 3. In Use

### a. The Diagram only

The diagram can be used by itself to represent the Valence brand where appropriate.

![The Diagram only](images/the-diagram-only.svg)
Download [SVG](#), [PNG](#)

### b. Wordmark only

The wordmark can be used by itself to represent the Valence brand where appropriate.

![Wordmark only](images/wordmark-only.svg)
Download [SVG](#), [PNG](#)

### c. Lockups

The Diagram and Wordmark can be locked up in two different ways. Horizontal lockup is preferred when there's limited surface amount to utilize. Vertical lockup is preferred for more official use.

![Horizontal lockup](images/horizontal-lockup.svg)
Download [SVG](#), [PNG](#)

![Vertical lockup](images/vertical-lockup.svg)
Download [SVG](#), [PNG](#)

## 4. Colors

### a. Brand colors

The red and blue of Valence primary colors are created using directly opposite colors in the HSL color space, each being shifted by 10 degrees. The red is adjusted to be 10° from zero degrees, representing a slight shift in hue from pure red. The blue color is also adjusted to be 10° away from 180 degrees, indicating the same shift from pure blue. The pure black is added to the set, making the three promary colors for Valence. These are the same colors used in the [blurred red circle](#a-blurred-red-circle), [black circle](#b-black-circle) and the overlapped area.

|                                                   | Name   | HSL             | RGB             | HEX       |
| ------------------------------------------------- | ------ | --------------- | --------------- | --------- |
| ![](https://placehold.co/15x15/FF2A00/FF2A00.png) | Red    | ` 10, 100,  50` | `255,  42,   0` | `#FF2A00` |
| ![](https://placehold.co/15x15/000000/000000.png) | Black  | `  0,   0,   0` | `  0,   0,   0` | `#000000` |
| ![](https://placehold.co/15x15/02D5FF/02D5FF.png) | Blue   | `190, 100,  50` | `  2, 213, 255` | `#02D5FF` |

![HSL Color Space](images/hsl-color-space.svg)

### b. Graphing colors

A separate set of colors, primarily to differentiate different categories shown in charts and graphs, is defined as below. These colors are chosen for their perceptual distinctiveness and verbal describability. 

The color set is also designed to be used in order. If you want only four colors, the first four colors from the list can be used, as the colors at the top of the list are more identifiable. It is best practice to keep the number of colors to a minimum in a single chart.

Please note that while the red is the same red as the brand color, but the blue is different for better legibility.

![Brand colors](images/graphing-colors.svg)

```js
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

The primary typeface for the Valence brand is Times, a classic typeface with a rich history. There are many digital variants of Times typeface, including Times (Linotype) included in macOS, and Times New Roman (Monotype) in Windows. While they are very similar and therefore interchangeable, the brand prefers Times (Linotype), the digitalized version of the typeface commissioned by the newspaper The Times.

The typeface can be used for brand messages and body text. However, for UI use, Times can be replaced with a font that has a slightly refined look, including Adobe Text Pro.

![Primary typeface](images/primary-typeface.svg)

### b. Secondary typeface

The secondary typeface, to be used in conjunction with the primary, is Unica 77 by Lineto. Unica 77 is versatile enough to be used in UI applications. The license for Unica 77 can be obtained from [Lineto website](https://lineto.com/typefaces/unica77?font=L3l-qxAYPaV).

![Secondary typeface](images/secondary-typeface.svg)

### c. Tertiary typeface

For a limited use, for visual clarity in numeric and code representation, the [monospaced variant of Unica 77](https://lineto.com/typefaces/unica77-mono?font=PDpITQJkbYI) can be used. Proper licenses to be obtained upon usage.

![Tertiary typeface](images/tertiary-typeface.svg)

## 6. Sample designs



## 7. Contact
For inquiries, please contact TKTK.
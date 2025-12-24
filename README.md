# Ex09 Event Registration Web Application
## Date: 24.12.2025
## Reference No: 25002753

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
page1
@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --colors-accents-blue: rgba(0, 136, 255, 1);
  --colors-backgrounds-primary: rgba(255, 255, 255, 1);
  --colors-fills-vibrant-tertiary: rgba(237, 237, 237, 1);
  --colors-labels-primary: rgba(0, 0, 0, 1);
  --colors-labels-vibrant-controls-primary: rgba(64, 64, 64, 1);
  --colors-labels-vibrant-primary: rgba(51, 51, 51, 1);
  --colors-labels-vibrant-secondary: rgba(153, 153, 153, 1);
  --large-title-emphasized-font-family: "SF Pro", Helvetica;
  --large-title-emphasized-font-size: 34px;
  --large-title-emphasized-font-style: normal;
  --large-title-emphasized-font-weight: 700;
  --large-title-emphasized-letter-spacing: 0.4000000059604645px;
  --large-title-emphasized-line-height: 41px;
}

/*

To enable a theme in your HTML, simply add one of the following data attributes to an HTML element, like so:

<body data-colors-mode="light">
    <!-- the rest of your content -->
</body>

You can apply the theme on any DOM node, not just the `body`

*/

[data-colors-mode="light"] {
  --colors-accents-blue: rgba(0, 136, 255, 1);
  --colors-backgrounds-primary: rgba(255, 255, 255, 1);
  --colors-fills-vibrant-tertiary: rgba(237, 237, 237, 1);
  --colors-labels-primary: rgba(0, 0, 0, 1);
  --colors-labels-vibrant-controls-primary: rgba(64, 64, 64, 1);
  --colors-labels-vibrant-primary: rgba(51, 51, 51, 1);
}

[data-colors-mode="dark"] {
  --colors-accents-blue: rgba(0, 145, 255, 1);
  --colors-backgrounds-primary: rgba(0, 0, 0, 1);
  --colors-fills-vibrant-tertiary: rgba(18, 18, 18, 1);
  --colors-labels-primary: rgba(255, 255, 255, 1);
  --colors-labels-vibrant-controls-primary: rgba(191, 191, 191, 1);
  --colors-labels-vibrant-primary: rgba(255, 255, 255, 1);
}

[data-colors-mode="IC-light"] {
  --colors-accents-blue: rgba(30, 110, 244, 1);
  --colors-backgrounds-primary: rgba(255, 255, 255, 1);
  --colors-fills-vibrant-tertiary: rgba(237, 237, 237, 1);
  --colors-labels-primary: rgba(0, 0, 0, 1);
  --colors-labels-vibrant-controls-primary: rgba(64, 64, 64, 1);
  --colors-labels-vibrant-primary: rgba(51, 51, 51, 1);
}

[data-colors-mode="IC-dark"] {
  --colors-accents-blue: rgba(92, 184, 255, 1);
  --colors-backgrounds-primary: rgba(0, 0, 0, 1);
  --colors-fills-vibrant-tertiary: rgba(18, 18, 18, 1);
  --colors-labels-primary: rgba(255, 255, 255, 1);
  --colors-labels-vibrant-controls-primary: rgba(191, 191, 191, 1);
  --colors-labels-vibrant-primary: rgba(255, 255, 255, 1);
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

PAGE2
@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

PAGE3
@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

```
## OUTPUT:
![013](https://github.com/user-attachments/assets/64be4458-e528-44d9-bf09-8c750e1a3c48)


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.

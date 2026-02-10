# ✨ Minimalist "Please Wait" Teaser Page

A sleek, modern loading page designed to build anticipation for a special event (February 14th). This page features a high-end CSS-animated loader, a gradient background, and a rhythmic "dots" animation to keep users engaged while they wait.

## 🚀 Live Preview
The page displays a glowing pink spinner against a deep space-themed gradient, with a soft reminder to return on **February 14th**.

## 🎨 Features

* **Anime-Style Loader:** A glowing, high-performance CSS spinner with a neon box-shadow effect.
* **Dynamic Typography:** Uses a "dots" animation (`...`) via CSS pseudo-elements to show the page is active.
* **Modern Aesthetics:** Deep 3-tone gradient background using `#0f2027`, `#203a43`, and `#2c5364`.
* **Fully Responsive:** Optimized for mobile, tablet, and desktop screens.
* **No Dependencies:** Built entirely with pure HTML and CSS—no external libraries or JavaScript required.

## 🛠️ Technical Breakdown

### CSS Animation: The Spinner
The loader uses a `spin` keyframe that rotates the element $360^\circ$ infinitely.


### CSS Animation: The Typing Dots
Instead of using JavaScript, the "loading dots" are handled via a CSS `@keyframes` targeting the `content` property of the `::after` pseudo-element:
```css
@keyframes dots {
  0% { content: ""; }
  25% { content: "."; }
  50% { content: ".."; }
  75% { content: "..."; }
}

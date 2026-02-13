# Valentine's Day Browser Game - Walkthrough

## Overview
A romantic, single-file browser game where you guide a character to find a heart. It features particle effects, smooth animations, audio synthesis, and a responsive design.

## Source Code
The source code is available on GitHub: [FarHanZzzz/valentines](https://github.com/FarHanZzzz/valentines)

## Features
- **Responsive Design**: Works on Desktop and Mobile.
- ** Jungle Theme**: A lush, green environment with stone blocks and grass.
- **Audio Synthesis**: Generates sound effects using Web Audio API (no external files).
- **Customizable**: Easy to change colors, messages, and the victory photo.
- **Single File**: Everything is contained in `index.html`.

## How to Play
1. **Open** `index.html` in any modern browser.
2. Click **Start Game** (this initializes the audio context).
3. Use **Arrow Keys**, **WASD**, or the **On-screen D-pad** (Mobile) to move the character (👧).
4. Navigate through the jungle maze to find the **Heart** (❤️) to win!

## Customization Guide
You can easily personalize this game for your Valentine by editing the `index.html` file.

### Change the Photo
Find the `<img>` tag in the `victoryScreen` div (around line 200) and replace the `src` URL:
```html
<!-- Replace this URL with your own photo URL -->
<img src="YOUR_PHOTO_URL_HERE" alt="Us" ...>
```

### Change the Message
Edit the text in the `victoryScreen` div:
```html
<h2>You Found My Heart! 💕</h2>
<!-- Change to: -->
<h2>Happy Valentine's Day, [Name]! 💕</h2>
```

### Change Colors
Edit the CSS Variables in the `<style>` section at the top of the file:
```css
:root {
    --soft-pink: #FFE5EC; /* Change background tint */
    --heart-red: #FF6B9D; /* Change heart color */
}
```

## Technical Details
- **Canvas API**: Used for rendering game entities and particles.
- **RequestAnimationFrame**: Ensures smooth 60fps animations.
- **AudioContext**: Synthesizes pleasant chimes and beeps in real-time.

# Museum of Impossible Things

A mysterious, responsive puzzle game built with React, TypeScript, and Vite. Explore a museum whose galleries do not follow ordinary rules: inspect strange exhibits, gather clues, solve mysteries, and uncover the room that has been watching you.

## Getting started

Requirements: Node.js 20 or newer and npm.

```bash
npm install
npm run dev
```

Vite prints a local URL when the development server is ready. To make and preview a production build:

```bash
npm run build
npm run preview
```

## How to play

1. Begin in the lobby and open the museum map.
2. Enter an available gallery and read its case file.
3. Click the exhibit’s inspection marker or drag the exhibit to inspect it for a clue. Use **Hint** for up to three graduated clues.
4. Enter your deduction in the case file. Solving an exhibit opens the next gallery.
5. Solve all three mysteries to reveal **The Museum That Is Looking At You**.

The current exhibits are:

- **The Impossible Staircase** — look for the landing that does not belong.
- **The Door to Yesterday** — find the year hidden in the museum’s past.
- **The Photograph That Changes** — notice the number concealed in the portrait.

## Controls and pages

- Use the sidebar to visit the lobby, museum map, collection, field notes, and settings.
- On smaller screens, use the menu button to open navigation.
- Select a gallery on the map to enter it. Locked galleries open as you solve mysteries.
- Click the exhibit marker to inspect it, or drag the exhibit within its display to reveal a clue.
- Toggle the theme with the sun/moon button in the top bar, or choose Dark or Light in Settings.

## Settings and saved progress

The game saves exhibit discoveries, solved mysteries, and settings in the browser’s `localStorage` under `museum-save-v1`. Settings include Dark/Light theme, sound effects, ambient music, and reduced motion. Use **Start over** in Settings to reset the save on this device.

Random museum events can reveal the **A Quick Look Away** collection discovery. You can also find a hidden visitor-badge interaction by clicking the visitor badge five times.

## Exhibit concepts

The museum’s concept list also includes **The Clock That Remembers Tomorrow**, **The Infinite Mirror**, and **The Living Shadow**. These are ideas for additional impossible exhibits; they are not playable in the current build.

## Project structure

```text
src/
  App.tsx       Museum navigation, exhibit puzzles, save data, and page content
  main.tsx      React application entry point
  styles.css    Responsive layout, themes, exhibit artwork, and animations
index.html      Vite HTML entry point
vite.config.ts  Vite and React configuration
```

## Accessibility and motion

The layout adapts to desktop and mobile widths. Interactive elements have accessible names, and the reduced-motion setting stops the museum’s random moving events. The app also respects the operating system’s reduced-motion preference.

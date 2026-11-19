# Space Wars

A 2D arcade space shooter in React and HTML5 Canvas. Dodge rocks, shoot UFOs, survive.

## What it does

- Start screen (Enter), game over screen, restart with `R`.
- Move with the arrow keys, fire with Space or the up arrow.
- Enemy ships and meteors spawn at random. Enemies shoot back.
- Hitting an enemy ship, a meteor or an enemy bullet ends the run.
- Score goes up every second you survive, and by 50 for each enemy you shoot.
- Bullets and meteors have hit animations, and the background scrolls.

## Stack

- React 19 (Create React App)
- HTML5 Canvas
- Sprites and fonts bundled in `src/assets` and `public/fonts`

## Run it locally

```bash
npm install
npm start    # http://localhost:3000
```

## Notes

Early project. Collision detection is plain bounding boxes in `src/utils/isCollision.jsx`, and game state lives in one large component (`src/app.jsx`). It imports `lodash/fp`, which is not listed in `package.json` and only resolves through Create React App's own dependencies. No score persistence, no sound, no levels.

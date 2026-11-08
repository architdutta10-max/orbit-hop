# 🪐 Orbit Hop

> A one-button arcade game in your browser. Orbit a planet, launch in a straight line, and get captured by the next one. Miss it and you drift into space.

![HTML5](https://img.shields.io/badge/HTML5-Canvas%20%7C%20Web%20Audio-orange)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-yellow)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Dependencies](https://img.shields.io/badge/Dependencies-None-brightgreen)
![Platform](https://img.shields.io/badge/Platform-Desktop%20%7C%20Mobile-lightgrey)

**▶ Play it:** https://architdutta10-max.github.io/orbit-hop/

---

## Overview

Orbit Hop is a single-file game built with plain HTML, Canvas and the Web Audio API. There are no frameworks, no assets and no build step. Everything, including the sound effects, is generated in code.

---

## How to Play

1. You start out circling a planet. A dotted line shows the direction you will fly.
2. **Tap, click, or press Space/Enter** to launch along that line.
3. Pass close to the next planet and its gravity captures you. You start orbiting it and score **+1**.
4. Miss, and you drift away. If you fly too far or too long, the run ends. Tap to retry.

**Tip:** your direction of spin depends on how you enter each orbit, so read every planet fresh. Release when the dotted line points at the next planet.

---

## Features

- **One-button controls**: works with mouse, touch and keyboard
- **Rising difficulty**: planets get farther apart as your score climbs
- **Generated sound effects** using the Web Audio API
- **Particle bursts, glowing trails and screen shake**
- **Best score saved** in your browser (`localStorage`)
- **Responsive**: scales to any screen size
- **Single file, zero dependencies, works offline**

---

## Run Locally

```bash
git clone https://github.com/architdutta10-max/orbit-hop.git
cd orbit-hop
```

Open `index.html` in any modern browser. No server needed.

---

## Deploy with GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under **Branch**, select `main` and `/ (root)`, then click **Save**
4. After a minute, the game is live at `https://architdutta10-max.github.io/orbit-hop/`

---

## Project Structure

```text
.
├── index.html     # The entire game (HTML + CSS + JS)
├── README.md      # This file
├── LICENSE        # MIT license
└── .gitignore     # Git ignore rules
```

---

## Tweaking the Game

Open `index.html` and look for these constants near the top of the script:

```js
const OMEGA=2.7, SPEED=330;   // orbit spin speed (rad/s) and launch speed (px/s)
```

The `mk()` function controls planet size and spacing, and the capture distance is `planet.R + 10`.

---

## Known Limitations

- Sound starts only after your first tap or click (a browser autoplay rule)
- The best score is stored per browser and does not sync between devices

---

## Roadmap

- [x] Orbit, launch and capture mechanic
- [x] Score, best score and restart
- [x] Sound effects and particle effects
- [ ] Moving planets
- [ ] Collectible stars
- [ ] Daily challenge with a fixed seed
- [ ] Online leaderboard
- [ ] Mute button

---

## Contributing

Pull requests are welcome. For major changes, please open an issue first.

1. Fork the repo
2. Create a branch (`git checkout -b feature/my-feature`)
3. Commit (`git commit -m 'Add my feature'`)
4. Push (`git push origin feature/my-feature`)
5. Open a Pull Request

---

## License

Released under the MIT License. Free for personal and commercial use. See [LICENSE](LICENSE) for the full text.

---

## Author

**Archit Dutta** · Siliguri, West Bengal, India

- 💼 **LinkedIn:** [in/archit-dutta-4522693aa](https://www.linkedin.com/in/archit-dutta-4522693aa/)
- 📸 **Instagram:** [@architdutta17](https://www.instagram.com/architdutta17/)
- 🐙 **GitHub:** [@architdutta10-max](https://github.com/architdutta10-max)
- ✉️ **Email:** architdutta10@gmail.com

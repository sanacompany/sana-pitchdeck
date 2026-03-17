# SANA Pitch Deck

Interactive pitch deck for **SANA** — an AI consulting & software development company.

**Live:** [sanacompany.io/sana-pitchdeck](https://sanacompany.io/sana-pitchdeck/)

## Overview

A single-page, slide-based presentation covering SANA's expertise across:

- AI / Research (Google DeepMind partnership, embodied AI)
- Robotics (EarthRovers, ROS/SDK, fleet operations)
- IoT & Maritime Intelligence (Tocaro Blue, Proteus)
- Games & Virtual Experiences (Wimbledon Hill, UEFA events)
- Crypto & Web3 (on-chain agents, token economies)

## Features

- Keyboard & touch navigation (arrow keys, space, swipe)
- EN / KR language toggle
- Smooth scroll-snap slide transitions with CSS animations
- Fully static — no build step required

## Tech Stack

- Vanilla HTML / CSS / JS
- Fonts: Bebas Neue, Cabinet Grotesk, General Sans
- Hosted via GitHub Pages

## Development

```bash
pnpm install
pnpm dev
```

Opens on `http://localhost:3000`.

## Project Structure

```
index.html          # Full presentation (markup + styles + scripts)
translations.json   # EN/KR content strings
assets/             # Images organized by section
  ai/
  brand/
  clients/
  crypto/
  games/
  iot/
  robotics/
```

## Deployment

Deployed automatically via GitHub Pages from the `main` branch.

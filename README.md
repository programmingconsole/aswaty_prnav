# Mohammed Shahal & Aysha Fasna — Nikah Invitation

A beautiful, premium, and fully responsive digital wedding/nikah invitation web application built using **React**, **TypeScript**, **Tailwind CSS**, and **TanStack Start**.

## Features

- **Elegant Aesthetics**: Sleek modern design featuring cream, gold, and maroon color tones, custom typography, animations, and background textures.
- **Audio Backdrop**: High-fidelity background music with a floating toggle button.
- **Falling Petals Animation**: Subtle and interactive falling rose petals across the screen.
- **Countdown Timer**: Real-time interactive countdown to the big day.
- **Interactive Details Card**: Smooth layout containing event times, details, and Google Maps navigation.
- **Vercel & Social Ready**: Optimized metadata for link sharing previews (Open Graph / WhatsApp / Telegram) with custom thumbnail previews.

## Tech Stack

- **Framework**: [TanStack Start](https://tanstack.com/router/v1/docs/start/overview) (Vite + React)
- **Styling**: Tailwind CSS
- **Icons**: Lucide Icons
- **Deployment**: Vercel

---

## Local Development

### 1. Installation

Install project dependencies using your preferred package manager (npm, bun, yarn):

```bash
npm install
# or
bun install
```

### 2. Run Development Server

Start the local server with hot-reloading:

```bash
npm run dev
# or
bun run dev
```

The application will run locally at `http://localhost:3000`.

### 3. Build & Production

Generate a static/serverless build optimized for Vercel production:

```bash
npm run build
```

You can preview the built production app locally using:

```bash
npm run preview
```

---

## Configuration & Customization

- **Wedding details & metadata**: Configured in [`src/routes/index.tsx`](file:///d:/DOWNLOADS/nikahsf/src/routes/index.tsx) and [`src/routes/__root.tsx`](file:///d:/DOWNLOADS/nikahsf/src/routes/__root.tsx).
- **Background Image**: Located at [`src/assets/nikah-bg.jpg`](file:///d:/DOWNLOADS/nikahsf/src/assets/nikah-bg.jpg).
- **Link Sharing Preview Thumbnail**: Located at [`public/thumbnail.jpg`](file:///d:/DOWNLOADS/nikahsf/public/thumbnail.jpg).
- **Backdrop Music**: Located at [`public/music1.mp3`](file:///d:/DOWNLOADS/nikahsf/public/music1.mp3).

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

### 1. How to Change Invitation Contents & Details

All the dynamic content (couple names, date, location, event time, and map links) is located in [`src/routes/index.tsx`](file:///d:/DOWNLOADS/nikahsf/src/routes/index.tsx).

- **Couple Names**: Update the text inside the `Cover` and `CardContent` components:
  - Cover Title: Modify the header text in the `Cover` function (around line 208).
  - Main Cards: Modify the `<h2>` tags under `{/* Couple */}` inside the `CardContent` function.
- **Date & Time Cards**: Locate the `{/* Date block */}` section (around line 290):
  - Left Card (Date): Update the text for Month, Day, Weekday, and Year.
  - Right Card (Time/Event): Update the time text (e.g. `11:30 AM`) and the subtitle text (e.g. `NIKAH CEREMONY`).
- **Countdown Target**: Inside the `CardContent` component, change the `<Countdown target="..." />` string property to your desired date and time in standard ISO format (e.g., `2026-08-29T11:30:00`).
- **Venue & Location Details**: Update the address text and Google Maps `href` link inside the venue block (around line 347).
- **Page Titles & Meta tags**: To change what is shown in the browser tab and search results, update the metadata arrays in both [`src/routes/index.tsx`](file:///d:/DOWNLOADS/nikahsf/src/routes/index.tsx) and [`src/routes/__root.tsx`](file:///d:/DOWNLOADS/nikahsf/src/routes/__root.tsx) (look for the `title` and `description` key-value pairs).

### 2. How to Add or Change Background Music

The invitation includes auto-playing ambient background music. To update the audio:

1. Prepare your new audio file in `.mp3` format.
2. Rename the file to `music1.mp3`.
3. Replace the existing file at [`public/music1.mp3`](file:///d:/DOWNLOADS/nikahsf/public/music1.mp3).
4. Run `npm run build` to package the updated assets for deployment.

### 3. How to Update Images

- **Background Wallpaper**: Replace the image located at [`src/assets/nikah-bg.jpg`](file:///d:/DOWNLOADS/nikahsf/src/assets/nikah-bg.jpg).
- **Link Sharing Preview Thumbnail**: Replace the file at [`public/thumbnail.jpg`](file:///d:/DOWNLOADS/nikahsf/public/thumbnail.jpg). This image is shown as the preview thumbnail when sending the website link over messaging apps like WhatsApp or iMessage.


# rceg_cegau

Lightweight frontend for the Rotaract Club of CEG — a TypeScript-first web app showcasing club events, media, and resources.

Why this repo
- Built for fellow developers and contributors: clean TypeScript codebase, modular CSS, and simple build scripts.
- Purpose: public site for events, galleries, and media shared by the club.

Tech stack (high level)
- TypeScript (primary language)
- CSS for styling
- JavaScript/HTML for small polyfills and embeds
- Typical tools: Node.js, npm/yarn, bundler (Vite/Next/your choice)

Quick start
1. Install Node.js (>=16) and npm or yarn
2. Clone the repo
   git clone https://github.com/Rotaract-club-of-CEG/rceg_cegau.git
3. Install dependencies
   npm install
4. Run locally
   npm run dev
5. Build for production
   npm run build

Project layout (typical)
- src/               — TypeScript source
- public/            — static assets (images, videos, favicons)
- public/assets/images/ — event photos and graphics
- public/assets/videos/ — short MP4/WebM clips (or placeholders)
- styles/ or src/styles — CSS modules / global CSS
- package.json       — scripts and deps

Images and videos (what to know)
- Where media should live
  - Store images in public/assets/images/ and videos in public/assets/videos/.
  - Keep filenames kebab-case and include a short JSON/MD manifest if you need metadata (credit, date, event).

- Where media come from (recommended text for site visitors & contributors)
  - Event photos and videos: primarily contributed by club members and event photographers.
  - Stock or supporting assets: use permissively licensed sources (Unsplash, Pexels, Pixabay) and list the source/credit in assets/CREDITS.md.
  - Embedded videos: use YouTube/Vimeo embeds only for official club channel links; do not hotlink random third-party uploads.

- Attribution & licensing
  - Add a file public/assets/CREDITS.md (or assets/CREDITS.md) listing: filename, source, author, license, and a short note (e.g., "photo: John Doe — Rotaract CEG event, 2025").
  - If you add stock imagery, include the exact Unsplash/Pexels URL and the photographer's name.
  - For any copyrighted media, ensure we have explicit permission before publishing.

Development notes
- Keep UI components small and typed. Prefer strict TypeScript settings for safety.
- Add new media via pull requests. PR checklist should include: media file(s) added to public/assets, updated CREDITS.md, and any size/optimization performed (e.g., responsive sources, WebP fallback).
- Optimize images: use responsive sizes and modern formats (WebP/AVIF) where possible.
- Videos: prefer short MP4 or H.264 for compatibility; provide poster images and lazy-loading.

Contributing
- Fork → branch → PR. Describe changes and include screenshots for UI work.
- Tests & linting: run linters and any unit tests before opening a PR.
- Code style: follow existing conventions; prefer descriptive commits.

Maintenance checklist for media-heavy site
- Regularly optimize new uploads (resize, compress).
- Periodically audit CREDITS.md for missing attributions.
- Remove or replace media for which permission is revoked.

Contact / Ownership
- Repository: Rotaract-club-of-CEG/rceg_cegau
- For media permission/contact, maintainers should keep a list of club photographers and rights holders in a private document.

License
- Add a LICENSE file or replace this section with the project license.

---

If you want, I can:
- create a starter public/assets/CREDITS.md file and add a contributing checklist template, or
- add example scripts (npm run dev/build) to package.json if you tell me which bundler/framework this repo uses.

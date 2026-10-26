---
status: pending
title: Hello World App
---

# Hello World App

A minimal single-page app that displays a friendly "Hello, World!" message on the home page, styled and centered on screen.

## Steps

1. **Create the global stylesheet at `src/styles/global.css`**
   - Must start with exactly `@import "tailwindcss";` so Tailwind CSS v4 utilities work across the app.
   - Expected outcome: Tailwind utility classes are available in every component.

2. **Create the app entry point at `src/main.tsx`**
   - Import `src/styles/global.css` once here.
   - Set up the TanStack Router with the generated route tree and render the app into the `#root` element in `index.html`.
   - Expected outcome: the app boots and the router controls what renders on screen.

3. **Create the root route / app shell at `src/routes/__root.tsx`**
   - Define the root route that renders an `<Outlet />` so child routes appear.
   - Expected outcome: every page in the app has a shared shell to render inside.

4. **Create the home route at `src/routes/index.tsx`**
   - Renders a full-screen, centered layout with a large "Hello, World!" heading and a short welcoming subline.
   - Use Tailwind classes for centering, typography and a pleasant background.
   - Expected outcome: visiting `/` shows "Hello, World!" centered on the page, looking clean on both mobile and desktop.

5. **Verify the app renders**
   - The home page loads without errors and the heading is visible.
   - Expected outcome: a working Hello World app ready for further features.

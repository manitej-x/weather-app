# Weather

Weather is a production-grade, installable weather app built in the `weather-pro` project folder.

The product direction is premium and motion-led: animated weather states, polished dark mode,
smooth scrolling, rich data visualization, geolocation, offline support, and an Android-ready PWA
install flow.

## Features

- Live weather search with autocomplete and recent locations.
- Current location support with approximate network fallback.
- Animated atmosphere scenes for sun, rain, snow, storm, mist, cloudy, and night conditions.
- Hourly temperature chart, seven-day forecast, and daily insight cards.
- Celsius/Fahrenheit switching, dark mode, loading states, retry states, and offline messaging.
- Installable Android PWA with manifest, service worker, app icons, and install prompt support.

## Commands

```bash
npm install
npm run dev
npm run lint
npm run format:check
npm run build
npm run preview
```

Use `npm run build` followed by `npm run preview` to test the production PWA locally. Service
workers only register in production builds.

## Architecture

- `src/app` owns app composition and providers.
- `src/components` contains reusable UI, animation, theme, and visual components.
- `src/config` contains application-level constants.
- `src/hooks` contains reusable React hooks for theme-independent browser state, online status, and
  PWA installation.
- `src/lib` contains framework-agnostic browser utilities.
- `src/pages` contains route-level screens.
- `src/styles` contains global Tailwind CSS setup.
- `src/types` contains shared TypeScript-only types.

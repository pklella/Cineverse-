# CineVerse Website

A React website prototype for discovering movies, series and anime, checking upcoming movie release dates, viewing available streaming providers, and saving a personal watchlist.

## Requirements

- Node.js 18 or newer
- A TMDB API key for movie and TV data
- Internet connection for live catalogue data and poster images

## Run locally

1. Extract this folder.
2. Open a terminal in the `cineverse-website` folder.
3. Run `npm install`.
4. Copy `.env.example` to `.env`.
5. Add your TMDB API key to `VITE_TMDB_API_KEY`.
6. Run `npm run dev`.
7. Open the local URL printed by Vite.

To create a production build, run `npm run build`.

## Data sources

- Movie and television metadata, release dates, images, ratings and watch-provider information: TMDB API.
- Anime listings and title details: Jikan API, which provides access to MyAnimeList data.

The website does not invent review counts, customer numbers, testimonials or engagement metrics. Release dates and streaming availability can change. Provider availability currently checks India first, then the United States as a fallback when the India result is not present. Update this region logic before public release if your audience is elsewhere.

## Prototype account storage

Registration, sign-in, session state and watchlist data use browser localStorage. This is only for a local prototype. Passwords are not securely hashed and there is no server-side authentication. Do not use real or reused passwords. Before public launch, replace this with a secure authentication backend, server-side validation, hashed passwords, session protection and a proper account recovery flow.

## Before public launch

- Connect and verify your custom domain.
- Configure HTTPS and production hosting.
- Review the Privacy Policy and Terms and Conditions with the actual operator details and data practices.
- Add a monitored contact email to the legal pages.
- Replace localStorage authentication with a secure backend.
- Review TMDB and Jikan attribution, branding, API usage and image rights requirements.
- Test all pages, links, forms, mobile layouts and API failure states.
- Remove any development-only configuration and keep API credentials out of public source control.

CineVerse is an independent prototype and is not endorsed or certified by TMDB.

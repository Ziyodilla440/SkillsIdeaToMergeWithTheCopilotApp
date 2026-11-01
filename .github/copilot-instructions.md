# Copilot instructions

Project context Copilot should apply to every session in this repository.

## Stack

- Framework: Astro (static output).
- Language: TypeScript.
- Styling: plain CSS in the base layout.

## Conventions

- Keep components small and focused.
- Prefer semantic HTML and accessible markup.
- Do not close, or add closing keywords for, the exercise walkthrough issue (issue #1) in any pull request. The exercise's GitHub Actions workflows manage that issue. When you open a pull request for app work, link only the specific app work-item issue you are implementing.

## Persistence and hydration rules

- **Persistence**: Bookmarks must be stored and persisted in the browser using `localStorage`.
- **Hydration**: All browser-only code accessing `localStorage` must run behind a client-side boundary using the `client:load` directive (or inside client-side `<script>` tags) so that Astro static site generation / SSR never touches browser APIs during build.

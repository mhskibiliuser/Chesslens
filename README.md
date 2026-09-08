# ChessLens

Browser-based chess analysis and training app.

## Included

- `index.html` — complete ChessLens app
- `data/GM.book` — GM opening book used by the bot and book-move detection
- `data/openings.json` — opening database used for theory/opening recognition

## Engine

ChessLens uses a single embedded Stockfish 17 Lite worker inside `index.html`, so the engine itself does not need a separate `.js` or `.wasm` download.

## Bolt.new

Import this repository into Bolt.new and use the repository root as the project root. The app should be served over HTTP/HTTPS so it can load the files under `data/`.

## Notes

Game analysis, review, and bot play share one Stockfish worker and are queued to avoid engine request collisions.

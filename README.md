# Durango Food Picker

A small personal web app that suggests where to eat in Durango, Colorado. You pick a mood, a cuisine, and a budget, and it ranks a hand-made list of 42 local restaurants by how well they match.

Plain HTML, CSS, and JavaScript in one `index.html`, plus a web app manifest and a service worker so it can be installed on a phone and opened offline. Hosted with GitHub Pages.

## How it works

1. Pick a mood (Comfort, Healthy, Indulgent, Adventure), a cuisine (Mexican, American, Italian, Asian, Fast Food, or Surprise), and a budget (cheap, moderate, splurge).
2. Each restaurant gets a score: +50 for a mood match, +35 for a cuisine match (+15 for Surprise), +15 for a budget match, plus a small bonus from its ratings.
3. Results are shown in score order.

The ratings (health, "gains", and cheapness, each 1–10) and the short notes on each restaurant are my own opinions, not official inspection grades or reviews.

## Run locally

```bash
python -m http.server 8000   # then open http://localhost:8000
```

## License

[MIT](LICENSE)

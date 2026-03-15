# SF Creative Events ✿

A curated list of creative events in San Francisco — workshops, exhibitions, craft fairs, and more.

🌸 **[Live site →](https://amywork777.github.io/sf-creative-events/)**

## Sources

- **TIAT** (The Intersection of Art & Technology) — [lu.ma/tiat](https://lu.ma/tiat) — 151 Powell St
- **nowplace 此间** — [lu.ma/nowplace](https://lu.ma/nowplace) — 679 Clay St
- **SF Junk Journal Club** — [@sfjunkjournalclub](https://www.instagram.com/sfjunkjournalclub/) on Instagram
- **SF Funcheap** — [sf.funcheap.com](https://sf.funcheap.com) — creative/craft/DIY events

## How to update events

Edit `public/events.json`. Each event has this structure:

```json
{
  "id": "unique-id",
  "title": "Event Name",
  "date": "2026-03-20",
  "endDate": "2026-03-21",       // optional, for multi-day events
  "time": "7:00 PM",
  "location": "Address, San Francisco",
  "price": "$30",                // or "Free" or "TBA"
  "source": "tiat",              // tiat | nowplace | junk-journal | funcheap
  "sourceName": "TIAT",          // display name for the source
  "link": "https://lu.ma/tiat",  // link to event/source page
  "description": "Short description of the event.",
  "recurring": "Every Wednesday"  // optional
}
```

Push to `main` and Vercel will auto-deploy.

## Tech

Static HTML/CSS/JS. No build step. Deployed on GitHub Pages (from `/docs` folder).

## Adding new sources

1. Pick a source key (e.g. `my-source`)
2. Add CSS variables in `index.html` for the source colors
3. Add a filter button in the HTML
4. Add events to `events.json` with the new source key

---

*curated with care ✿*

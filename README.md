# The Weekly Hallucination

An AI & tech weekly — written by a machine with no bias whatsoever. Published every Monday at
https://mervikki.github.io/The-Weekly-Hallucination/ (it ran as *The Daily Hallucination* from May 11 to September 23, 2026).

Written and published by a GitHub Copilot automation that follows [`editorial/prompt.md`](editorial/prompt.md).

| Path | What it is |
| --- | --- |
| `index.html` | Archive page (weekly issues first, then the daily archive) |
| `weekly/YYYY-MM-DD.html` | Weekly issues, dated by their Monday |
| `daily/YYYY-MM-DD.html` | The 135 daily issues (frozen, never edited) |
| `assets/issue.css` | Shared stylesheet for weekly issues |
| `templates/` | Issue, special-issue and chart skeletons used by the automation |
| `editorial/prompt.md` | The publishing prompt the automation runs |
| `editorial/memory.md` | Editorial memory, read and updated every run |
| `editorial/memory-archive.md` | Retired memory entries (not read during a run) |
| `404.html` | Redirects old root-level daily URLs to `daily/` |

## Requesting a special issue

A special issue is a two-page edition: page 1 is only about one big AI event, page 2 is the rest of the week.
The editor decides on its own when an event qualifies (see `editorial/prompt.md` → *Special issues*). To force one,
commit `editorial/special-request.md` to `main` before the Monday run, e.g.:

```markdown
Event: OpenAI releases GPT-7
Why: first model to pass X; I want the full front page on it.
```

The next run publishes the special and deletes the file.

# xRay

**Advanced X.com query constructor** — build powerful search queries visually with a terminal-style interface. No frameworks, no dependencies, no build step — just open the HTML file.

![Zero Dependencies](https://img.shields.io/badge/dependencies-0-brightgreen?style=flat-square)
![Single File](https://img.shields.io/badge/size-1%20file-brightgreen?style=flat-square)

![xRay Screenshot](xray-redesign.png)

## Features

- **Visual query builder** — fill in fields, get a properly formatted search query in real-time
- **Keywords** — all words, exact phrase, any of (OR), excluded words, hashtag
- **Account filters** — from, to, mentioning, exclude account, from list
- **Date range** — since/until date pickers
- **Engagement minimums** — min likes, retweets, replies
- **Links & sources** — filter by URL domain or source app
- **Content filters** — images, videos, media, links, verified only, replies only, quote tweets, safe mode, has question, exclude retweets/replies
- **Language filter** — 30+ languages supported
- **One-click search** — opens the query directly on X.com
- **Copy to clipboard** — grab the raw query string
- **Save & load searches** — persisted in localStorage, survives browser restarts
- **Search history** — automatically tracks recent searches
- **Templates** — pre-built queries for common use cases (viral tweets, threads, popular media, discussions, etc.)
- **Operators cheatsheet** — built-in reference tab for all supported search operators
- **Smart query parsing** — loading a saved search populates the individual fields back

## Usage

Open `twitter-search.html` in any modern browser. That's it.

1. Fill in the fields on the left panel
2. Watch the query build in real-time on the right
3. Click **Search X.com** to run it, or **Copy Query** to grab it
4. Optionally save searches for later with a label

## Query Operators Reference

| Field | X Search Operator | Example |
|-------|-----------------|---------|
| All words | (space-separated) | `bitcoin market` |
| Exact phrase | `"..."` | `"mass adoption"` |
| Any of | `OR` | `(bitcoin OR ethereum)` |
| Exclude words | `-word` | `-scam -giveaway` |
| Hashtag | `#tag` | `#bitcoin` |
| From account | `from:` | `from:elonmusk` |
| To account | `to:` | `to:jack` |
| Mentioning | `@user` | `@vitalikbuterin` |
| Exclude account | `-from:` | `-from:spambot` |
| From list | `list:` | `list:123456` |
| Since date | `since:` | `since:2024-01-01` |
| Until date | `until:` | `until:2024-12-31` |
| Min likes | `min_faves:` | `min_faves:100` |
| Min retweets | `min_retweets:` | `min_retweets:50` |
| Min replies | `min_replies:` | `min_replies:10` |
| URL contains | `url:` | `url:github.com` |
| Source app | `source:` | `source:Twitter_Web_App` |
| Language | `lang:` | `lang:en` |
| Exclude RTs | `-filter:retweets` | |
| Images only | `filter:images` | |
| Videos only | `filter:videos` | |
| Has media | `filter:media` | |
| Has links | `filter:links` | |
| Verified only | `filter:verified` | |
| Replies only | `filter:replies` | |
| Exclude replies | `-filter:replies` | |
| Quote tweets | `filter:quote` | |
| Safe mode | `filter:safe` | |
| Has question | `?` | |

## Why?

X.com's built-in advanced search is buried and clunky. xRay gives you a fast, keyboard-friendly interface to construct complex queries without memorizing operator syntax.

## License

MIT

[Русский 🇷🇺](README_ru.md) / **English 🇺🇸**

# Dashboard as a Product

**Product:** interactive map of a product approach to BI  
**Role:** Product Manager / Author  
**Context:** 18 artifacts and 17 processes with examples for Power BI, Tableau, Looker

**Result:** BI as a product — artifacts, processes, and maturity, not just «draw some charts».

**Site:** [addito-5g.github.io/Dashbord-as-product](https://addito-5g.github.io/Dashbord-as-product/)

![Project UI](dashboard.png)

---

## Structure

```
├── index.html           — React app
├── data-artifacts.js    — 18 artifacts (4 layers)
├── data-processes.js    — 17 processes (6 phases)
└── assets/              — ~100 PNGs
```

## Run locally

```bash
python3 -m http.server 8080
# → http://localhost:8080
```

## Contributing

Card copy lives in `data-artifacts.js` and `data-processes.js`. Card fields:

```js
{
  n: 1,
  name: "Product Vision",
  short: "...",
  detail: `...`,      // markdown
  dashboard: `...`,
  bi: `...`,
  maturity: "mvp",    // mvp | growth | mature
}
```

Images: `assets/`, prefixes `a01-`…`a18-`, `p01-`…`p17-`. Recommended width — 1024px PNG.

> Edit `index.html` only when display logic changes.

# Shijie Zhou — personal website

Static academic homepage based on [Jon Barron's template](https://github.com/jonbarron/jonbarron.github.io). No build step.

- `index.html` — all content (one `<tr>` per paper; highlighted rows use `bgcolor="#ffffd0"`)
- `stylesheet.css` — Barron's stylesheet plus a few additions at the bottom (hover thumbnails, mobile layout)
- `images/` — profile photo, favicon, paper thumbnails (`<key>.jpg`; optional `<key>_hover.jpg` shown on mouse-over)
- `data/CV_Shijie_Zhou.pdf` — CV linked from the header

Preview locally:

```sh
python3 -m http.server 8000   # then open http://localhost:8000
```

Not deployed yet. To publish later with GitHub Pages: push this folder to the repo `shijiez37.github.io` under the GitHub organization `shijiez37` (site URL: https://shijiez37.github.io).

## Visitor analytics (private)

`index.html` ends with an invisible [Statcounter](https://statcounter.com) snippet (project 13363580, already configured). Nothing is shown on the page; only you see the stats in the Statcounter dashboard.

1. Sign up at statcounter.com → **Add Project** with the site's public URL.
2. Choose the **invisible** counter, then copy `sc_project` and `sc_security` from the generated code.
3. Paste them into the two variables at the bottom of `index.html`.

Until both are filled in, the snippet does nothing. It also skips `localhost` and `file://` previews. In the dashboard, **Recent Visitor Activity** lists each visit with time, country/city, ISP/organization, referrer, and pages viewed. To keep your own visits out, use **Settings → Blocking Cookie**.

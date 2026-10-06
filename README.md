# voltforge.tech

Forwards `https://voltforge.tech/thor-tigress-cub` (and every other path) to
the Thor Tigress Cub, which the Jetson AGX Thor serves itself at
`https://arpanpathak.taildb9a39.ts.net/`.

This repository holds no UI and no data: each page only sends the browser on.
GitHub Pages provides the HTTPS certificate for `voltforge.tech`, so both hops
are HTTPS. Why it is built this way: the book, chapter "Bring your own domain"
(https://arpanpathak.github.io/thor-thunder-tigress-platform/ch17-bring-your-own-domain.html).

| File | Purpose |
|---|---|
| `CNAME` | tells GitHub Pages the domain |
| `index.html`, `thor-tigress-cub/index.html` | forward to the Thor |
| `404.html` | forwards any other path too |
| `.nojekyll` | serve the files as they are |

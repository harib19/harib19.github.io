# harib19.github.io

Personal site. One file, no build step, no dependencies.

## Deploy on GitHub Pages (free)

1. Repo (under the harib19 org) is named exactly `harib19.github.io`
2. Push `index.html` to the `main` branch
3. Settings → Pages → Source: **Deploy from a branch** → `main` / `root`
4. Live at `https://harib19.github.io` in a minute or two

```bash
git init
git add index.html README.md
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/harib19/harib19.github.io.git
git push -u origin main
```

## Custom domain (optional, ~₹800/year)

Buy a domain, then add a file named `CNAME` containing just your domain
(e.g. `haribhaskaran.com`). Point these A records at GitHub:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Then Settings → Pages → Custom domain → enter it → tick **Enforce HTTPS**.

## Editing

Everything is in `index.html`. Colours are CSS variables at the top under
`:root`. Light and dark both defined; the Theme button overrides the
system preference and remembers the choice.

To add a project, copy one `<div class="row">` block inside `.list`.
To add a paper, copy one `<article class="paper">` block.

# Connor's Workflow Guide
## Summer Web Agency — How to Pull and Review Sites

---

## Getting the Latest Version of Any Site

Whenever Owen pushes new work, open VS Code, open the terminal with **Ctrl + `** and run:

```
git pull origin main
```

This downloads the latest version instantly.

---

## How to Preview a Site in Your Browser

In the VS Code terminal type:

```
start index.html
```

The site opens in your browser. Go through it fully — test every section, check it on your phone by opening the Vercel link, and flag anything that looks off.

---

## Current Sites to Review

**Coffee Shop Sample**
- GitHub: https://github.com/OwenWUher/coffeeshop-sample
- Live: https://coffeeshop-sample.vercel.app
- Already cloned to your laptop at `Documents/coffeeshop-sample`

To get the latest version:
1. Open VS Code
2. File → Open Folder → Documents → coffeeshop-sample
3. Open terminal with **Ctrl + `**
4. Run `git pull origin main`
5. Run `start index.html` to preview

---

## How to Push Your Edits Back to Owen

When you make changes in VS Code and want to send them back:

```
git add .
```

```
git commit -m "describe what you changed"
```

```
git push
```

The live Vercel site updates automatically every time either of you pushes.

---

## Your Role
- Pull Owen's latest builds and review them in VS Code
- Open sites in your browser and test everything — links, buttons, mobile view, forms
- Make small edits directly in VS Code (text changes, color tweaks, placeholder swaps)
- Push your fixes back to GitHub
- Flag anything broken or off before it goes to a client

---

*Questions? Ask Owen.*

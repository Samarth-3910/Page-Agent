# Page Agent Showcase

This is a small demo site I built for Page Agent, an open source library by Alibaba that lets you control a webpage using plain English instead of clicking around.

It's just one HTML file. No build tools, no npm install, nothing complicated. Open it and it works.

## What it does

There's a fake signup form and a small checklist on the page. Instead of filling them in yourself, you type something like "set the plan to Pro and turn off marketing updates" into the box and it does it for you. It's using Page Agent's free demo API in the background so you don't need your own API key to try it.

## Running it locally

Just double click index.html or open it in your browser. That's it.

## Putting it on GitHub Pages

If you want to host this yourself:

1. Make a new repo on GitHub.
2. Push these files to it:

```
git init
git add .
git commit -m "add page agent demo site"
git branch -M main
git remote add origin https://github.com/your-username/your-repo.git
git push -u origin main
```

3. In the repo, go to Settings, then Pages.
4. Under Source pick "Deploy from a branch", set branch to main and folder to root, then save.
5. Wait a minute or two and your site will be up at:

```
https://your-username.github.io/your-repo/
```

## Notes

- Heads up: the free demo LLM runs through Alibaba's infrastructure in China. Anything you type into the command box, plus the page content it reads to act on it, gets sent there. Don't type in real names, emails, passwords, or anything sensitive when trying the demo, just use fake data. Read the full docs and terms before relying on this for anything beyond testing: https://alibaba.github.io/page-agent/docs/features/models#free-testing-api
- The demo LLM is free but it's meant for testing only, it's shared and rate limited so don't expect it to be fast every time.
- If you want to use your own model instead of the free one, there's a code snippet on the site itself under "Get started" showing how to swap in your own API key.
- This isn't official, just a fan project, not made by or connected to Alibaba.

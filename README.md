[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/takoyakimaru333/site-generator-speed-01/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/takoyakimaru333/site-generator-speed-01/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

# sitegen-fast

A fast drop-in for makefun-site 1.0.0, written for the make.fun bounty
[site-generator-speed-01-run-20261122](https://make.fun/competitions/site-generator-speed-01-run-20261122):
for every case it returns, byte for byte, the output tree makefun-site 1.0.0
builds — each page's `index.html`, the index and tag pages, `build-report.txt`
and each static file — only faster.

`solve.js` is a dependency-free ES module exporting `run(input)`. It is an
original implementation of makefun-site's own front matter, template dialect,
Markdown subset, slug rule and report, written from the behaviour its README
describes: Markdown renders straight to HTML, inline text is escaped in whole
runs, and templates are compiled once into small functions instead of being
walked as trees on every page. `main.ts` is the harness driver: it reads
`/input/cases.json`, answers each case alone with `run`, and writes
`/output/answers.json`.

---

<sub>Entered on [make.fun](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) · AI agents build software for cash rewards</sub>

---
description: Fast portfolio update - batched price fetches, auto-update from screenshots (project)
---

Portfolio update for index.html. Do everything automatically with minimal prompting.

1. Open wealthsimple.com, then watch ~/Downloads for new *.png files (poll every 3s, up to 3 min). Wait a few extra seconds after the first screenshot appears in case more are coming.
2. Read all screenshots and extract:
   - Cash balances (Vacation chequing, TFSA cash)
   - Any stock/ETF positions: symbol, shares, current price, daily % change
3. If stock positions exist, WebSearch each tradeable symbol to cross-reference prices. Flag >2% difference; prefer WebSearch price if screenshot looks stale.
4. WebSearch "CAD to USD exchange rate" and calculate USD total.
5. Update index.html:
   - Update cash balances in Portfolio section
   - Update USD total in Portfolio tfoot
   - Add/update/remove stock position rows as needed
   - If holdingsConfig JS exists, update fallbackPrice and fallbackDailyChange
   - Update "Last updated" date
6. git commit, git push, open index.html in Chrome
7. Delete processed screenshots from ~/Downloads

No emojis, no questions, minimal output. Just do it.

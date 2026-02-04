---
description: Suggest portfolio rebalancing based on current prices and targets
---

Analyze the portfolio and suggest rebalancing.

No emojis. No AI-speak. No m-dashes. Be direct and concise.

1. Read current holdings from index.html (shares, current prices, target prices)
   - If no stock positions exist, skip rebalancing and just report cash balances.
2. Calculate current allocation vs target allocation
3. Identify positions that are overweight, underweight, or at target
4. Consider market conditions, upcoming earnings, tax implications, transaction costs

Provide specific recommendations:
- Sell X shares of [STOCK] at $Y to realize Z% gain
- Buy X shares of [STOCK] at $Y to reach target allocation
- Hold [STOCK] (at target)

Format as a clear action list with reasoning. Keep it factual and straightforward.

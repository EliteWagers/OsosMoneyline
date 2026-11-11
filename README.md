# Elite Wagers Picks Center

This rebuild changes the site into a sports-picks dashboard: moneyline markets, player props where the provider supports them, game scores, a pick tracker, and an optional AI matchup explainer.

## Deploy on Render
- Runtime: Node
- Root Directory: blank
- Build Command: `npm install`
- Start Command: `npm start`
- Instance: Free for initial testing

Upload every file in this ZIP directly to the root of your GitHub repository, replacing the old versions.

## API keys
1. Create a free account at https://the-odds-api.com/ and get an API key.
2. In Render, open your Web Service → Environment → Add Environment Variable.
3. Name: `THE_ODDS_API_KEY`; Value: your key. Save and redeploy.
4. Free access is limited (currently listed as 500 credits/month on the provider's pricing page); the exact sports/markets and usage costs depend on the provider's current plan. Free access is suitable for prototyping, not a full paid picks service.
5. Optional: add `OPENAI_API_KEY` and `OPENAI_MODEL=gpt-5-mini` to enable AI explanations. OpenAI API usage is billed separately; ChatGPT subscription does not include API credits.

## Data honesty and commercial launch
- Odds are sportsbook market prices. The dashboard derives market-implied probabilities; these are not independently validated win predictions.
- Player props are only returned when the provider and plan support that sport/market. The free Odds API tier may not include props.
- ESPN scoreboard JSON is unofficial and can change. Check provider/league data rights before charging subscribers or redistributing feeds.
- Before launching paid subscriptions, add user accounts, Stripe billing, server-side access control, a paid/free entitlement system, pick history and grading, customer support, privacy/terms/refund pages, and responsible-gambling disclosures. Confirm every data provider permits commercial display/redistribution on your chosen plan.
- Do not advertise “guaranteed” picks or claim a historical hit rate until picks are timestamped, independently graded, and reported with sample size and ROI.

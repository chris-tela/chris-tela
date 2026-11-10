# Mid-Tier and Budget NBA Stats API Providers: Pricing and Terms (as of Nov 2026)

> **Method caveat (read first):** Every direct page fetch failed. balldontlie.io, mysportsfeeds.com, api-sports.io and sportsdata.io would not resolve because the session network does not allow them, so the other provider sites were not tried. All findings below come from **web-search result summaries and snippets**. They are not verified page reads. Treat each price as "reported by the search index for this URL" and re-confirm it on the live page before budgeting. Where results conflicted, both values are shown. To verify, allow these hosts in the session network settings: balldontlie.io, mysportsfeeds.com, api-sports.io, sportsdata.io, goalserve.com, rolling-insights.com, thesportsdb.com and rapidapi.com.

## What are the exact published prices and tier limits for each provider as of 2026?

### Takeaway
Only a few providers publish self-serve NBA prices: balldontlie ($0 / $9.99 / $39.99 per month), API-Sports API-NBA (free 100 req/day, then roughly $10–$35/mo) and Goalserve ($150–$250/mo for basketball, $1,200–$1,500/yr). SportsDataIO's self-serve Discovery Lab tier ($99–$149/mo) is personal-use only. SportsDataIO commercial, MySportsFeeds commercial and Rolling Insights are quote-based. Third-party estimates put SportsDataIO commercial at $500–$1,000+/mo.

### Cited Findings

**balldontlie (balldontlie.io)**
- The official account/plans endpoint lists three NBA tiers: free at $0/mo with 5 req/min, ALL-STAR at $9.99/mo with 60 req/min, and GOAT at $39.99/mo with 600 req/min — [balldontlie account page](https://www.balldontlie.io/account/); the tier names come from [SportIntel MCP config guide](https://glama.ai/mcp/servers/@roizenlabs/sportintel-mcp/blob/f8a45ddbbee2feb94796eb7a42efcac559a0b05b/docs/deployment/CONFIGURE_API_KEY.md)
- Tiers are bought per sport, so an NBA subscription does not cover other balldontlie sports — [sportsapis.dev review](https://sportsapis.dev/apis/balldontlie)
- ALL-STAR ($9.99) adds active players, player injuries and the stats endpoint. GOAT ($39.99) adds box scores, live box scores, game lineups, play-by-play, and odds/props — [balldontlie.io](https://balldontlie.io); [sportsapis.dev](https://sportsapis.dev/apis/balldontlie)
- The free tier covers basic endpoints only. Stats, box scores and odds need a paid plan — [sportsapis.dev](https://sportsapis.dev/apis/balldontlie); [BallDontLie limitation doc](https://glama.ai/mcp/servers/@roizenlabs/sportintel-mcp/blob/f8a45ddbbee2feb94796eb7a42efcac559a0b05b/docs/development/BALLDONTLIE_LIMITATION.md)
- Trial length conflicts: one review says a 7-day GOAT trial, while a StackOne guide shows a 48-hour GOAT trial banner — [sportsapis.dev](https://sportsapis.dev/apis/balldontlie); [StackOne guide](https://docs.stackone.com/connectors/balldontlie/guides/link-account/api-key)
- Jentic says balldontlie has no paid tier, which conflicts with the official plans and is likely outdated — [Jentic](https://www.jentic.com/apis/balldontlie)

**API-Sports (API-NBA / API-Basketball)**
- Direct from api-sports.io (API-NBA): free gets 100 req/day. Paid tiers are PRO (7,500/day), ULTRA (75,000/day) and MEGA (150,000/day), reported at about $15, $25 and $35/mo. The quota resets at 00:00 UTC and unused requests are lost — [api-sports.io NBA page](https://api-sports.io/sports/nba)
- On RapidAPI (API-Basketball): Basic is free with 100 req/day, a 10 req/min limit and $0.0005 per extra request. Pro is $10/mo for 7,500/day, Ultra $15/mo for 75,000/day and Mega $20/mo for 150,000/day — [RapidAPI api-basketball pricing](https://rapidapi.com/it/api-sports/api/api-basketball/pricing)
- The RapidAPI API-NBA listing shows different numbers, for example Pro at $15/mo for 5,000/day. Figures vary by listing and date — [RapidAPI api-nba pricing](https://rapidapi.com/de/api-sports/api/api-nba/pricing)
- A RapidAPI collection calls the RapidAPI API-NBA listing "a limited version" — [RapidAPI NBA stat collection](https://rapidapi.com/hi/collection/nba-stat-api)
- Getting-started guide for API-NBA — [api-football.com blog](https://www.api-football.com/news/post/how-to-get-started-with-api-nba-the-complete-beginners-guide)

**Goalserve**
- NBA/NCAA live data (English prices page): $250 for 1 month, $900 for 6 months, $1,500 for 12 months — [Goalserve NBA prices](https://www.goalserve.com/sport-data-feeds/nba-api/prices)
- "Basketball Live Score" package (Italian page): $150/mo, $700 for 6 months, $1,200 for 12 months. It covers 100+ leagues with live scores, standings and historical data — [Goalserve IT](https://goalserve.com/it/sport-data-feeds/nba-api/prices)
- US Sports Package (NBA/NCAA + NFL + MLB + NHL): $400/mo, $1,850 for 6 months, $3,100 for 12 months. A French page shows a $2,500/yr promo plus "one extra year free" on yearly subscriptions — [Goalserve FR](https://goalserve.com/fr/sport-data-feeds/nba-api/prices)
- A competitor blog quotes Goalserve's All Sports plan at $425/mo billed annually. That does not match Goalserve's own pages, so it is unreliable — [sportsapi.com blog](https://sportsapi.com/blog/posts/affordable-sports-apis-for-developers)
- Goalserve says its feeds can be used in "livescore, fantasy applications, betting and more" — [Goalserve NBA samples](https://goalserve.com/es/sport-data-feeds/NBA-api/samples)

**SportsDataIO / FantasyData**
- FantasyData's commercial API division was rebranded as SportsDataIO in 2019. SportsDataIO is a subsidiary of FantasyData LLC, so this was a rebrand, not a merger — [SBC Americas 2019](https://sbcamericas.com/2019/04/18/fantasydata-confirms-rebrand-of-its-commercial-api-division/); [SportsDataIO company](https://sportsdata.io/company)
- The FantasyData NBA API docs now point to SportsDataIO Discovery Lab for hobbyists and to the SportsDataIO commercial NBA API for larger projects — [FantasyData NBA docs](https://developers.fantasydata.com/api-documentation/nba); [FantasyData vs SportsDataIO](https://FantasyData.com/fantasydata-api-vs-sportsdataio-api)
- Discovery Lab: Fantasy or Odds is $99/mo or $599/yr, and Fantasy + Odds is $149/mo or $899/yr. A free tier is also listed. Data is real but delayed to the next day — [SportsDataIO Discovery Lab](https://discoverylab.sportsdata.io/); [sportsapis.dev review](https://sportsapis.dev/apis/sportsdata-io)
- A third-party source reports Discovery Lab daily caps of 100–1,000 calls depending on tier (unverified) — [apis.io rate limits](https://apis.io/rate-limits/sportsdataio/sportsdataio-rate-limits/)
- Free trial: self-serve, no credit card, all endpoints and sports, but returns **scrambled** data. Scores and game stats are randomly shifted by 5–20%; schedules, teams and players are not — [SportsDataIO getting started](https://sportsdata.io/developers/getting-started); [Scrambled data help](https://sportsdata.io/help/scrambled-data)
- Commercial real-time pricing is not public; SportsDataIO says to contact sales for a custom proposal — [SportsDataIO getting started](https://sportsdata.io/developers/getting-started)
- Third-party estimates disagree. Highlightly's 2026 roundup says $500–$1,000+/mo to start; a 2025 betting-API guide says a $250/mo base with $500–$2,000/mo for higher tiers; another blog says "from ~$19/mo" — [Highlightly 2026](https://highlightly.net/blogs/best-nba-apis-in-2026); [The Sports Economist 2025](https://thesportseconomist.com/?p=19194); [api.market blog](https://api.market/blog/recodex/allsportsapi/best-sports-api)
- Vendr hosts a pricing-intelligence listing for SportsDataIO (contents not retrieved) — [Vendr](https://vendr.com/marketplace/sportsdataio)

**MySportsFeeds**
- The official pricing page says plans start "at $49 per month for CORE feeds and Non-Live access". It is free for developers, students and hobbyists doing non-commercial work. Add-on prices vary with access level and multi-month term — [MySportsFeeds pricing](https://www.mysportsfeeds.com/feed-pricing/)
- Datarade says MySportsFeeds has not published full pricing and to contact the vendor — [Datarade](https://datarade.ai/data-providers/mysportsfeeds/profile)
- A 2016 Reddit post said non-commercial started at about $10/mo and that commercial pricing depended on post-game vs live (**outdated, 2016**) — [r/iOSProgramming 2016 (mirror)](https://axebps-redlib.hf.space/r/iOSProgramming/comments/4p6nzd/affordable_sports_data_api_postgame_or_live)
- Highlightly calls its pricing model "modular", so costs grow as you add feeds — [Highlightly 2026](https://highlightly.net/blogs/best-nba-apis-in-2026)

**Rolling Insights / DataFeeds**
- A Slashdot comparison lists DataFeeds at $50/month and a "Post Game & Real Time Sports Data API" starting at $4,200. It doesn't say which sports or terms apply (unverified) — [Slashdot](https://slashdot.org/software/comparison/OddsPapi-vs-Rolling-Insights/)
- DataFeeds is described as real-time and post-game feeds for all major North American sports, with a 30-day free trial on registration — [implexa listing](https://implexa.ai/s/clawhub/sports-datafeeds-by-rolling-insights)
- Rolling Insights is an FSGA (Fantasy Sports & Gaming Association) member — [FSGA directory](https://members.thefsga.org/member-directory/Details/rolling-insights-2558291)
- A Basketball DataFeeds listing also exists on Zyla Labs (price not shown in results) — [Zyla Labs](https://www.zylalabs.com/api-marketplace/top-search/Basketball%20-%20DataFeeds%20by%20Rolling%20Insights)

**TheSportsDB**
- Livescores are a Premium (V2) feature, updated every 2 minutes and sent with an X-API-KEY header — [TheSportsDB docs/about](https://www.thesportsdb.com/docs_about)
- SourceForge lists premium at $6. Whether that is the current Patreon price is unverified — [SourceForge](https://www.sourceforge.net/software/product/TheSportsDB)
- The site is community-run and funded by premium users and donations. Upgrades can be refunded within 14 days — [TheSportsDB terms (mirror)](https://backiee.wasmer.app/http_www_thesportsdb_com/docs_terms_of_use_php)

**Others surfaced**
- Fantasy Nerds offers an NBA API that includes depth charts — [Fantasy Nerds NBA docs](https://api.fantasynerds.com/docs/nba)
- Fine Print Analytics sells NBA data through RapidAPI plans — [Fine Print Analytics](https://fineprintanalytics.github.io/api.html)
- Apify NBA scraper actors are priced from $0.01 per 1,000 results. They scrape data, so licensing is questionable — [Apify NBA actor](https://apify.com/alizarin_refrigerator-owner/nba-api---basketball-statistics/pricing)
- Sportradar, the enterprise benchmark, has custom pricing; its fantasy tier includes pre-calculated fantasy points — [sonictechpro](https://www.sonictechpro.com/blog/best-sports-data-apis-for-fantasy-sports-apps/)

### Inferences
- For a small season-long fantasy startup, the cheapest self-serve paths with live box scores are balldontlie GOAT (about $480/yr) and API-Sports (about $120–$420/yr). Goalserve ($1,200–$1,500/yr) is the cheapest published price from a vendor that markets explicitly to fantasy apps.
- The SportsDataIO $99–$149/mo Discovery Lab price is **not** usable for a public app, so the real SportsDataIO cost is the commercial quote.
- API-Sports prices differ between its direct site and RapidAPI, so check both. Direct API-NBA and RapidAPI API-Basketball are separate products.

### Gaps
- None of the official pricing pages could be read directly, so every price is unconfirmed by a page read.
- I found no current MySportsFeeds commercial or live add-on price, and no Rolling Insights NBA-specific price.
- Tank01 (RapidAPI) pricing did not appear in any search results.
- I could not confirm TheSportsDB's current Patreon premium price.

## Which tiers allow commercial use in a public app (vs. personal/non-commercial only)?

### Takeaway
SportsDataIO is explicit: Discovery Lab and the free trial are personal and non-commercial only, and any public or revenue-generating product needs a commercial license. MySportsFeeds' free and low tiers are non-commercial, with commercial pricing separate. Goalserve markets its feeds for fantasy apps. I found no commercial-use terms for balldontlie or API-Sports. API-Sports' sister terms put league IP compliance on the customer.

### Cited Findings
- SportsDataIO: Discovery Lab is licensed only for personal, non-commercial use. Public-facing, revenue-generating or business-operated products need a commercial license — [SportsDataIO data rights & licensing](https://sportsdata.io/help/data-rights-and-licensing-questions)
- FantasyData.com API users are "generally individuals seeking data for their own personal models." SportsDataIO is the B2B arm, with clients such as FanDuel, The Athletic and Microsoft — [FantasyData vs SportsDataIO](https://FantasyData.com/fantasydata-api-vs-sportsdataio-api)
- MySportsFeeds is free for developers, students and hobbyists doing non-commercial work; commercial is priced separately — [MySportsFeeds pricing](https://www.mysportsfeeds.com/feed-pricing/); [2016 Reddit (outdated)](https://axebps-redlib.hf.space/r/iOSProgramming/comments/4p6nzd/affordable_sports_data_api_postgame_or_live)
- Goalserve says its feeds suit "fantasy applications, betting and more" — [Goalserve NBA samples](https://goalserve.com/es/sport-data-feeds/NBA-api/samples)
- The API-Sports sister site (api-football.com) terms say some sports data may be subject to IP or commercial restrictions imposed by leagues or organizers, and the customer is responsible for compliance — [api-football.com terms](https://www.api-football.com/terms)
- Searches found no balldontlie terms covering commercial use — [search on balldontlie.io](https://balldontlie.io)
- Yahoo's Fantasy Sports API requires the attribution "Fantasy data provided by Yahoo Fantasy" and has its own API terms. It serves league data, not a raw stats feed — [Yahoo developer](https://sports.yahoo.com/developer/); [Yahoo Fantasy API ToS](https://legal.yahoo.com/us/en/yahoo/terms/product-atos/fantasysportsapi/index.html)
- The unofficial nba.com stats endpoints can break overnight without warning — [XScanHub 2026](https://www.xscanhub.com/articles/best-nba-api-2026-comparison)

### Inferences
- A public, monetized fantasy app needs a written commercial grant. Only SportsDataIO (commercial license) and the quote-based vendors (MySportsFeeds commercial, Rolling Insights, Goalserve) are clearly set up for this. balldontlie and API-Sports should be asked in writing before launch.
- Fantasy use of player stats is generally treated differently from betting or official-data licensing. Even so, sources say little about the official vs. self-collected origin of budget providers' data.

### Gaps
- I found nothing on balldontlie's ToS, API-Sports' own ToS, TheSportsDB's commercial clause, or Rolling Insights' license terms.
- Data source (official NBA feed vs. self-collected or scraped) is undocumented in the results for every budget provider.
- I found no information on headshot or image rights for any provider.

## How fast are live stat updates (seconds vs. minutes) and how are stat corrections handled?

### Takeaway
SportsDataIO documents the most: with a real-time plan, clients can poll every 3–5 seconds, box scores run about 15–20 seconds behind the broadcast, season aggregates refresh every 10–15 minutes, and corrections should be re-pulled for 24–72 hours after a game. TheSportsDB livescores update every 2 minutes. balldontlie, API-Sports, Goalserve and MySportsFeeds latency figures were not found.

### Cited Findings
- SportsDataIO: real-time subscribers can sync scores and box scores every 3–5 seconds; the API caches responses, so polling faster adds little — [SportsDataIO refresh rates](https://sportsdata.io/help/refresh-rates-feeds-and-timing)
- SportsDataIO box scores update "15-20 seconds behind broadcast" — [SportsDataIO content update frequency](https://sportsdata.io/developers/content-update-frequency)
- SportsDataIO season stats refresh every 10–15 minutes for the NBA — [SportsDataIO refresh rates](https://sportsdata.io/help/refresh-rates-feeds-and-timing)
- Corrections: refresh box scores for at least 24 hours after a game, ideally 48–72 hours, and run a nightly pull covering the past 3–4 days — [SportsDataIO integration guide](https://sportsdata.io/help/sports-data-integration-guide)
- Resulting guide: results are re-run every 2 hours for 72 hours after the initial result — [SportsDataIO resulting guide](https://sportsdata.io/help/resulting-guide); [Game lifecycle](https://sportsdata.io/help/game-lifecycle)
- One guide says SportsDataIO's paid Scores API runs under 5 seconds, which is fine for fantasy but not live betting — [api.market blog](https://api.market/blog/recodex/allsportsapi/best-sports-api)
- TheSportsDB premium livescores update every 2 minutes — [TheSportsDB docs](https://www.thesportsdb.com/docs_about)
- Discovery Lab data is delayed to the next day — [sportsapis.dev](https://sportsapis.dev/apis/sportsdata-io)
- For comparison, Sportradar documents variable cache and update frequencies per endpoint, plus push feeds — [Sportradar update frequencies](https://developer.sportradar.com/basketball/docs/update-frequencies); [Sportradar push](https://developer.sportradar.com/basketball/docs/nba-ig-push)
- ESPN fantasy documents its own stat-correction policy, a useful benchmark for user expectations — [ESPN stat corrections](https://support.espn.com/hc/en-us/articles/360000099732-Stat-Corrections)

### Inferences
- Season-long fantasy rarely needs sub-minute latency. A 1–2 minute delay is acceptable, but stat-correction handling (re-pulling 24–72 hours of games) matters more for final scoring.
- On balldontlie the rate limit is a practical constraint on live polling. Free (5/min) and ALL-STAR (60/min) can't poll a full NBA slate's live box scores often, which is effectively why GOAT exists.

### Gaps
- I found no documented live latency or stat-correction policy for balldontlie, API-Sports, Goalserve, MySportsFeeds or Rolling Insights.

## What do developers say about accuracy, downtime, and support?

### Takeaway
Independent developer reviews are thin. Searches returned no Reddit or HN threads, and most sources are vendor or comparison blogs. The consensus is SportsDataIO for a serious fantasy product, MySportsFeeds for startup budgets, and balldontlie for hobby or single-sport use. Budget vendors are described as fine for an MVP but behind tier-one providers on depth, latency and reliability.

### Cited Findings
- SportsDataIO is called the leader for fantasy data, with DFS projections, season-long projections and DFS-specific data — [apisports.net](https://www.apisports.net/best/fantasy-sports-apis); [sonictechpro](https://www.sonictechpro.com/blog/best-sports-data-apis-for-fantasy-sports-apps/)
- MySportsFeeds is described as fitting "US-sports fantasy apps on startup budgets" — [api.market blog](https://api.market/blog/recodex/allsportsapi/best-sports-api)
- One developer integration log saw balldontlie stats calls take 10–30 seconds and needed caching (a single anecdote) — [SportIntel balldontlie integration notes](https://glama.ai/mcp/servers/@roizenlabs/sportintel-mcp/blob/f8a45ddbbee2feb94796eb7a42efcac559a0b05b/docs/development/BALLDONTLIE_INTEGRATION_SUCCESS.md)
- Smaller providers, SportsDataIO and MySportsFeeds included, are "viable for MVPs" but generally don't match tier-one providers on depth, latency or reliability — [Kanopy Labs 2026](https://kanopylabs.com/blog/how-to-build-a-fantasy-sports-app)
- Highlightly says SportsDataIO offers one of the deepest NBA datasets — [Highlightly 2026](https://highlightly.net/blogs/best-nba-apis-in-2026)
- Chrome Web Store reviews exist for an extension built on API-NBA (contents not retrieved) — [NBA Daily extension](https://chrome.google.com/webstore/detail/nba-daily/eplagjpgcidlidnopgeakefijdkjjjbd/reviews)

### Inferences
- Many "comparison" blogs are written by competing vendors (Highlightly, sportsapi.com, SportsGameOdds), so treat their rankings as marketing.

### Gaps
- I found no Reddit (r/webdev, r/sportsanalytics, r/fantasybball) or Hacker News threads; searches returned none.
- I found no published uptime or SLA figures for any budget provider.

## What do known indie fantasy apps use?

### Takeaway
Not answered. Searches found no public statements on which data vendors Fantrax, Sleeper, Yahoo or indie fantasy basketball tools license.

### Cited Findings
- Sleeper has a public read-only JSON API for league and player data, but its underlying stats vendor isn't named — [Zuplo Sleeper API](https://zuplo.com/learning-center/sleeper-api)
- Yahoo's API requires "Fantasy data provided by Yahoo Fantasy" attribution, with no outside vendor named — [Yahoo developer](https://sports.yahoo.com/developer/)
- Hobby fantasy basketball tools on GitHub, such as a fantasy simulation project, use balldontlie — [fea-game hoop data notes](https://fea-game.github.io/hoop/archived/fantasy-simulation/3-data)
- SportsDataIO names FanDuel, The Action Network, The Athletic and Microsoft as clients — [FantasyData vs SportsDataIO](https://FantasyData.com/fantasydata-api-vs-sportsdataio-api)
- RotoBaller's 2026 media kit advertises B2B data/API services, a possible alternative source of projections and news — [RotoBaller media kit](https://www.rotoballer.com/wp-content/uploads/2026/08/RotoBaller-Media-Kit-B2B-Services-and-APIs.pdf)

### Gaps
- Which vendors Fantrax, Sleeper, ESPN, Yahoo and indie apps use is unconfirmed; it may need vendor customer pages or press releases.
- Projections, news and headshots by tier: only SportsDataIO (projections in Fantasy feeds) and balldontlie (injuries on ALL-STAR) were confirmed. I found nothing on news or headshots for any budget provider.

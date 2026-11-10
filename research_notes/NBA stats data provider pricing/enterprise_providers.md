# Enterprise / Official NBA Data Providers: Pricing & Terms for a Small Season-Long Fantasy Startup

> Research date: 2026-11-10. **Method caveat:** this session's network blocked direct page fetches (developer.sportradar.com, sportsapis.dev, news.ycombinator.com all failed DNS). Every finding below comes from search-engine result summaries/snippets of the cited pages, not full-page reads. Treat specific numbers as "reported by the cited page" and verify before relying on them. Separately, most "price" figures for Sportradar come from **competitor marketing pages**, which have an incentive to make Sportradar look expensive.

## 1. What does Sportradar's NBA API cost for a commercial startup? Trials, startup tiers, reported quotes, contract terms and usage restrictions

### Takeaway
Sportradar publishes **no prices**. Every production contract is a custom quote through sales. The only self-serve option is a free trial key: 30 days, 1,000 calls, 1 QPS, one sport per key, not licensed for production, and without Push (real-time) feeds. Reported starting prices range from about $500–$1,250/month (directory estimates) to $10k+/month (a competitor's claim, mostly about odds feeds). A small fantasy startup should expect a four-to-five-figure annual minimum at least. The best route to cheap access is the Acceleradar startup program, which historically gave up to a year of free "Core" (non-real-time) data to young, low-funding US startups.

### Cited Findings
**Published (official Sportradar) info**
- Trial keys default to a 30-day period, a quota of 1,000 requests per rolling 30 days, and 1 query/second. Some images and editorial trials have smaller quotas, and larger limits require contacting sales. — [Sportradar Getting Started: Your Account](https://developer.sportradar.com/getting-started/docs/your-account)
- Each trial key covers a single sport and is capped at 1,000 calls per rolling 30 days. — [Sportradar Tennis v2 FAQ](https://developer.sportradar.com/tennis/v2/docs/faqs). The golf FAQ says trial keys last **90 days**, which conflicts with the 30-day default and may be product-specific or outdated. — [Sportradar Golf v2 FAQ](https://developer.sportradar.com/golf/v2/docs/faqs)
- Registration and trial flow: production access is reserved for Sportradar customers, and the trial is for evaluation. — [Sportradar Registration](https://developer.sportradar.com/getting-started/docs/registration)
- NBA Push feeds (real-time Push Clock, Events, Statistics, Draft) are an **add-on** that is "unavailable in the self-issued NBA trial" and limited to "Sportradar Realtime customers." — [Sportradar NBA Push integration guide](https://developer.sportradar.com/basketball/docs/nba-ig-push); [NBA Push Feeds reference](https://developer.sportradar.com/basketball/reference/nba-push-feeds)
- **Acceleradar (startup program):** launched in 2016 as a free program giving early-stage, **US-based** startups free sports data for **up to one year**. Eligibility at launch: companies no more than one year old with ≤$500,000 in funding. It covers non-third-party "Core" data API access, **not** the real-time feed (official and third-party data), and includes mentorship and coaching. — [TCB Mag: Sportradar Launches Acceleradar (2016)](https://tcbmag.com/sportradar-launches-aacceleradara-free-program-for-sports-tech-startups/); [FSGA: Sportradar Introduces Acceleradar](https://thefsga.org/sportradar-introduces-acceleradar). Later cohorts are documented, e.g. Blocksport in 2020-21. — [blocksport.io](https://blocksport.io/?p=36717). Acceleradar has its own terms and conditions page. — [Sportradar Acceleradar T&Cs](https://developer.sportradar.com/sportradar-updates/page/acceleradar-terms-and-conditions). *Eligibility criteria are from 2016. I found no current official criteria.*

**Licensing terms (official Sportradar documents, partial)**
- Sportradar's Official Data licence is described as "revocable, non-exclusive, limited," and use of rights-holder IP requires approval. — [Sportradar terms page](https://sportradar.com/?p=10377)
- The Official Media Data Addendum grants a "limited, revocable, worldwide, non-sublicensable and nontransferable" licence. Creating new or derivative data points needs Sportradar's written approval. — [Sportradar Official Media Data Addendum](https://developer.sportradar.com/Official_Media_Data_Addendum)
- Sportradar special terms bar use of league or tournament logos and player imagery without permission. — [Sportradar Special Terms & Conditions](https://sportradar.com/special-terms-conditions/)
- A Sportradar US Master Terms & Conditions page exists (developer.sportradar.com/terms-and-conditions), but its text was not retrievable. **Caching rules, display-only clauses and contract minimums could not be confirmed.** — [Sportradar developer T&Cs](https://developer.sportradar.com/terms-and-conditions)

**Reported / anecdotal pricing (NOT published by Sportradar)**
- SharpAPI (a competitor) claims Sportradar contracts are custom-negotiated, "typically starting in the five-figure range per month" for **odds feeds**, and elsewhere says "$10,000+/month." This is biased marketing and refers to betting/odds, not fantasy stats. — [SharpAPI: Sportradar alternative](https://sharpapi.io/compare/sportradar-alternative)
- A search summary attributes "Custom API plan from $1,250/month" for Sportradar to a 2026 directory page. — [SportsAPI.com Sportradar listing](https://sportsapi.com/api-directory/sportradar/). *Snippet-level only, unverified.*
- Another 2026 guide says Sportradar uses custom enterprise pricing, "typically $500–5,000+/mo." — [MoneyLine: 12 Best Sports Data APIs 2026](https://www.moneylineapp.com/blog/best-sports-apis) *(snippet attribution; possibly from the Sonictechpro or LSports guides returned in the same query)*
- A directory rates Sportradar at its top "$$$$$" price tier, defined as $1,000+/mo. — [sportsapis.dev Sportradar review 2026](https://sportsapis.dev/apis/sportradar)
- **Hacker News (2016, old):** a commenter who used Sportradar called it too expensive, said the data is occasionally wrong, and described the developer experience as weak. Another commenter suggested a $25/month consumer-style competitor could win the market Sportradar prices out. — [HN item 11837102](https://news.ycombinator.com/item?id=11837102)
- Onboarding is reportedly slow because data licence agreements with leagues are involved. — [sportsapis.dev Sportradar review](https://sportsapis.dev/apis/sportradar)
- Sportradar is described as best suited to large fantasy platforms and regulated real-money operators, with strengths in official data and low latency. — [Sonictechpro: Top 10 Live Data APIs for Fantasy](https://www.sonictechpro.com/blog/best-sports-data-apis-for-fantasy-sports-apps/)
- The only publicly listed enterprise sports-data contract price found anywhere is LSports' TRADE360 at $180,000 for 12 months on AWS Marketplace. That is a betting/trading product, retrieved July 2026 per an LSports guide. — [LSports: How Much Does Sports Data Cost in 2026](https://www.lsports.eu/blog/sports-data-cost)

### Inferences
- The figures span roughly $500 to $10k+ per month because they describe different products: core stats with delayed push versus real-time odds or official betting data. For a season-long fantasy app, which needs no sub-second latency, the realistic Sportradar scenario is a "Core" (non-Push) NBA package. Its cost is likely at the low end of the enterprise range, but it is still a negotiated annual contract.
- Season-long fantasy needs only final or near-live box scores, which Sportradar's pull API already provides. Paying for the Realtime/Push add-on is probably unnecessary.
- The trial cannot legally power a launched product, because production use requires a customer agreement.
- If the startup is young and lightly funded, Acceleradar is the most cost-effective way into Sportradar data. Its current eligibility should be confirmed with Sportradar.

### Gaps
- No verified, recent (2025–2026) firsthand quote from a founder, Reddit thread or HN post for Sportradar NBA fantasy pricing. Reddit searches returned nothing indexed.
- Minimum contract length, caching/storage rights and redistribution clauses in Sportradar's master terms could not be read because of the network block. Annual contracts are typical in the industry, but I found no source specific to Sportradar NBA.
- Whether Acceleradar is still accepting applicants in 2026 and its current criteria.

## 2. What exactly does the Sportradar–NBA exclusive deal restrict?

### Takeaway
Since 2023-24, the November 2021 deal has made Sportradar the **exclusive worldwide distributor of the NBA's *official* data** (NBA, WNBA, G League) through 2030-31, including official betting data, streaming and expanded tracking-data rights. It controls the league's own official feed. It does **not**, and legally could not, stop other companies from independently collecting and selling NBA box-score statistics. US courts have held that game scores and statistics are public facts (NBA v. Motorola, 1997), and fantasy use of player names and stats is protected (C.B.C. v. MLBAM, 2007). Non-official providers such as SportsDataIO and Stats Perform continue to sell NBA stats for fantasy.

### Cited Findings
- From the 2023-24 season, Sportradar is the exclusive worldwide provider of NBA, WNBA and NBA G League data. The deal also expanded its rights to player tracking data. Uses cited include new products and support for betting operators' and **media partners'** use of the data. — [Sportradar IR: NBA and Sportradar announce landmark long-term global partnership (Nov 2021)](https://investors.sportradar.com/news-releases/news-release-details/nba-and-sportradar-announce-landmark-long-term-global); [SEC Form 6-K exhibit](https://www.sec.gov/Archives/edgar/data/1836470/000119312521331929/d261556dex991.htm)
- The term runs from 2023-24 through the 2030-31 season. — [SportBusiness: Sportradar, FanDuel extend NBA data pact through 2030-31](https://sportbusiness.com/news/sportradar-fanduel-extend-nba-data-agreement)
- The NBA received a ~3% equity stake. Reports disagree on the structure: warrants vesting over eight years per [Yahoo Sports](https://sports.yahoo.com/nba-grabs-3-data-giant-125318714.html), versus ten years per [Legal Sports Report](https://www.legalsportsreport.com/59545/nba-ownership-stake-sportradar/).
- Reported deal values conflict: ~$1B per [SportsPro, citing Sportico](https://www.sportspro.com/news/betting/nba-sportradar-betting-data-streaming-equity-worth/), ">$1B in cash and stock" per [TheStreet](https://www.thestreet.com/investing/sportradar-1-billion-dollars-nba-data-distribution-deal), and >$3B per [Gaming Today, citing SBJ](https://www.gamingtoday.com/news/nba-sportradar-exclusive-data-rights-equity-deal/).
- Before the deal, Sportradar and Genius Sports held **non-exclusive** US rights to distribute official NBA/WNBA betting data (2018, extended 2020). Operators wanting official data had to go through one of them. — [NBA PR: first betting data partnerships (2018)](https://pr.nba.com/nba-betting-data-partnerships-sportradar-genius); [NBA PR: extension (2020)](https://pr.nba.com/nba-sportradar-genius-sports-group-partnerships); [Legal Sports Report](https://www.legalsportsreport.com/26353/nba-announces-betting-deals/)
- Trade reporting says Genius failed to win a comparable exclusive deal. Sportradar "wins exclusive NBA data rights from 2023-24." — [next.io](https://next.io/?p=10767) *(headline only)*
- Sportradar also supplies FanDuel with official NBA data through 2030-31. — [iGaming Business](https://igamingbusiness.com/sports-betting/sportradar-scores-long-term-nba-data-deal-with-fanduel)
- **Legal background:** in NBA v. Motorola (2d Cir. 1997), the NBA lost its copyright claims against a pager service that relayed scores and stats gathered by non-NBA reporters. Facts are not copyrightable, though the court left a narrow "hot news" misappropriation theory open. — [CCBJ: Who Has Title to Statistics](https://ccbjournal.com/articles/who-has-title-statistics); [UBC IP Law blog (Nov 2025)](https://iplaw.allard.ubc.ca/2025/11/17/is-sports-data-copyrightable-exploring-copyright-protection-in-sport-betting/)
- In C.B.C. Distribution v. MLBAM (E.D. Mo. 2006; 8th Cir. 2007), the court held that players' names and statistics used in fantasy games are not copyrightable and that the First Amendment outweighs players' publicity claims. CBS Interactive v. NFLPA later applied this to fantasy football. — [CommLawBlog](https://www.commlawblog.com/2007/10/articles/intellectual-property/major-league-baseball-strikes-out-in-attempt-to-prevent-use-of-player-information-by-fantasy-leagues/); [Sports Litigation Alert](https://sportslitigationalert.com/fantasy-sports-and-the-right-of-publicity/); [Techdirt](https://archive.techdirt.com/articles/20071016/143318.shtml)
- SportsDataIO, a non-official provider, publishes full NBA coverage for 2025-26 and sells fantasy plans. — [SportsDataIO 2025-26 NBA Confirmed Coverage](https://sportsdata.io/nba-confirmed-coverage)

### Inferences
- The exclusivity matters mainly for (a) regulated **betting** operators, many of whose state regulators or operator policies require "official league data" for in-play markets; (b) the league's raw, fastest in-arena feed and optical tracking data; and (c) use of NBA marks and logos, plus the "official" label. A season-long fantasy app needs none of these.
- Using NBA/team logos, the "official" branding, or league-supplied photos still requires a licence (NBA Properties, or the NBPA for group player-likeness deals), whatever the stats source. Stats and names alone are low-risk under C.B.C.
- I found no evidence that Sportradar's exclusivity has been used to stop unofficial stats vendors from selling NBA data to fantasy apps.

### Gaps
- The full contractual text of the NBA–Sportradar deal is not public. The precise carve-outs for "fantasy" and "media" are unknown.
- NBA.com's own terms on scraping stats.nba.com were outside this scope; another researcher may cover them.

## 3. What do Stats Perform (Opta) and Genius Sports offer for NBA fantasy, and at what reported prices?

### Takeaway
**Stats Perform** sells a dedicated fantasy product: stats, projections, news and widgets for season-long, DFS, best ball and dynasty formats. It covers the NBA, has powered DraftKings, and says it works with startups. Pricing is quote-only, and I found no reported dollar figures. **Genius Sports** is primarily a betting/official-data company. It lost out on NBA exclusivity, and I found no evidence of an NBA fantasy-stats product or pricing aimed at startups. It is not a realistic option for this use case.

### Cited Findings
**Stats Perform / Opta**
- Stats Perform's fantasy data supports "season-long leagues, daily fantasy sports (DFS), best ball, and dynasty formats," with pre-game, live and post-game stats, APIs and widgets for live stats and player profiles, and fantasy-specific projections, expected points and advanced metrics. — [Stats Perform Fantasy FAQs](https://www.statsperform.com/faqs/stats-perform-faqs-fantasy/)
- The Fantasy Content product lists player statistics, projections, news and personalised player performance recaps. — [Stats Perform: Fantasy Content](https://www.statsperform.com/products/fantasy-content/)
- Pricing: no public plan prices. "Products and pricing are tailored to meet the requirements of large and small enterprise-level clients," custom licensing is available by competition, country or data level, and the FAQ says Stats Perform "works with many startups and smaller organisations." — [Stats Perform Pricing & Licensing FAQs](https://www.statsperform.com/faqs/stats-perform-faqs-pricing-licensing/); [alt FAQ page](https://www.statsperform.com/stats-perform-faqs-pricing-and-licensing/)
- Third-party view: custom enterprise licensing, trial access on request, low affordability rating, "may be prohibitive for smaller organizations." This review is aimed at team-analytics buyers. — [FitGap: Stats Perform](https://us.fitgap.com/products/024574/stats-perform); [FitGap: Opta](https://us.fitgap.com/products/opta)
- DraftKings extended its DFS data deal with Stats Perform in 2020, covering the NBA, MLB, NHL and WNBA among others. — [Business Wire (June 2020)](https://www.businesswire.com/news/home/20200629005587/en); [Stats Perform press](https://www.statsperform.com/press/draftkings-extends-deal-with-stats-perform-to-boost-daily-fantasy-sports-experience)
- In November 2025, Stats Perform launched an Opta basketball "Dynamic Stats" API aimed at personalised prop betting. — [SBC Americas (Nov 2025)](https://sbcamericas.com/2025/11/19/stats-perform-basketball-api/)
- Stats Perform says its feeds deliver sub-second latency for live scoring (vendor claim). — [Stats Perform FAQ](https://www.statsperform.com/faqs/stats-perform-faqs-fantasy/)
- A developer knowledge base exists. — [developers.statsperform.com](https://developers.statsperform.com/)

**Genius Sports**
- Genius held non-exclusive US official NBA betting data rights in 2018 and 2020, alongside Sportradar. — [NBA PR (2020)](https://pr.nba.com/nba-sportradar-genius-sports-group-partnerships)
- Genius held an overseas NBA betting data deal reported as 6 years / $250M (2016). I found no evidence of renewal. — [Bloomberg](https://www.bloombergquint.com/business/nba-breaks-fresh-ground-for-sports-with-first-gambling-data-deal)
- Sportradar became exclusive from 2023-24, and Genius did not secure similar exclusivity. — [next.io](https://next.io/?p=10767)
- Genius owns Second Spectrum (acquired for ~$200M), the optical tracking firm. — [Sports Handle](https://sportshandle.com/nba-sportradar-exclusive-partnership-sports-betting-data/)
- Genius's documented basketball fantasy work is with Australia's NBL (FIBA LiveStats powering the NBL fantasy product), not the NBA. — [iGaming Business](https://igamingbusiness.com/sports-betting/genius-scores-data-extension-with-australias-national-basketball-league/)

**Other "enterprise-lite" provider (for comparison)**
- SportsDataIO lists self-serve Fantasy at $99/mo or $599/yr and Fantasy + Odds at $149/mo or $899/yr. It says the self-serve tiers are **not licensed for commercial redistribution**, and that commercial fantasy platforms need a sales conversation with pricing by use case, volume and sports. — [SportsDataIO Developers](https://sportsdata.io/developers); [SportsDataIO Data Rights & Licensing help](https://sportsdata.io/help/data-rights-and-licensing-questions) *(snippet-level; verify current prices)*
- LSports says custom pricing is the norm across the industry. — [LSports blog](https://www.lsports.eu/blog/sports-data-cost)

### Inferences
- For a season-long fantasy startup, Stats Perform is the only enterprise competitor to Sportradar with an off-the-shelf fantasy package that includes projections and news. Whether it is cheaper is unknown without a quote.
- Genius Sports should be deprioritised: its NBA business centres on betting, tracking and media, it does not hold the official NBA data rights, and no fantasy-startup product turned up.
- SportsDataIO's commercial-licence requirement suggests that even "mid-market" vendors push commercial fantasy apps off self-serve plans into negotiated contracts.

### Gaps
- No reported dollar quotes for Stats Perform or Genius NBA fantasy feeds.
- Whether Genius currently sells any NBA stats product to non-betting media or fantasy customers in the US.
- I found no reliable published uptime/SLA figures for any provider.

## 4. Do injury news, projections and headshots come bundled or cost extra? (Plus coverage, latency and reliability)

### Takeaway
At Sportradar, injuries are part of the NBA stats API (a Daily Injuries feed). Headshots come from a **separate Images API**, with premium transparent headshots as an extra package and some photos under Getty terms. Real-time Push is a paid add-on. I found no Sportradar NBA projections product. At Stats Perform, projections and news are part of the fantasy content offering. At SportsDataIO, headshots are a separate News & Images feed. Exact bundle pricing is unpublished everywhere.

### Cited Findings
- The Sportradar NBA v8 API includes a Daily Injuries feed ("details for all injuries updated on a given date"), alongside complementary feeds. — [Sportradar NBA v8 docs](https://developer.sportradar.com/docs/read/basketball/NBA_v8); [NBA overview](https://developer.sportradar.com/basketball/v7/reference/nba-overview)
- Sportradar's Images API v3 (a separate product) serves player headshots, venue images, logos and action shots. Transparent headshots require an extra Premium package for select sports, and images require following 302 redirects. Some photographs fall under Getty Images licence terms. — [Sportradar Images API v3](https://developer.sportradar.com/images-and-editorials/reference); images trials have smaller quotas per [Your Account](https://developer.sportradar.com/getting-started/docs/your-account)
- NBA Push feeds (low-latency) are an add-on for Realtime customers only. — [Sportradar NBA Push](https://developer.sportradar.com/basketball/docs/nba-ig-push)
- An NBA/NCAAMB release log documents ongoing API changes. — [Sportradar changelog](https://developer.sportradar.com/sportradar-updates/changelog/nba-ncaamb-apis)
- Stats Perform's fantasy content includes projections, news and recaps. — [Stats Perform Fantasy Content](https://www.statsperform.com/products/fantasy-content/)
- SportsDataIO lists headshots under a separate News & Images product. Its 2024 coverage PDF shows headshots as a separate feed. NBA projections include injury monitoring, DFS salaries and projected stats. — [SportsDataIO News & Images](https://sportsdata.io/news-and-images); [Headshots API](https://sportsdata.io/developers/sports-player-headshots-api); [SDio Coverage PDF](https://sportsdata.io/files/SDio_Coverage.pdf); [Boomi SportsData NBA v3 Projections](https://help.boomi.com/docs/Atomsphere/Connect/MCPConnectors/sportsdata-nba-v3-projections)
- Reliability reputation (anecdotal): HN, 2016: Sportradar "data is occasionally wrong" and the developer experience is weak. — [HN](https://news.ycombinator.com/item?id=11837102). 2026 comparison guides credit Sportradar with official data and low latency. — [Sonictechpro](https://www.sonictechpro.com/blog/best-sports-data-apis-for-fantasy-sports-apps/)

### Inferences
- Budget headshots as a separate line item from any enterprise vendor. Player imagery also raises publicity and photo-licence issues (Getty, NBA Properties) that a pure stats licence does not cover.
- Projections are likely an extra or separate product. Sportradar does not appear to sell NBA fantasy projections, so a startup using Sportradar may need a second vendor or in-house projections.
- Latency is largely irrelevant for season-long fantasy, since minute-level or post-game updates suffice. Paying for official, sub-second data buys little.

### Gaps
- No published add-on prices for Sportradar Images, Push or Injuries.
- No independent uptime/SLA data, and no recent (2024–2026) developer reliability reports for any of the vendors.
- Whether Sportradar's Images licence permits use in a commercial fantasy app without additional NBA/NBPA licensing.

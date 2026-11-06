## Aurelix: clean, tested web data tools

Aurelix builds web data tools on the [Apify Store](https://apify.com/aurelix) for **jobs, e-commerce, lead generation, ad research and public records**. Every tool is built to do one job well, at a fair price.

**The problem we solve:** you need public web data (job postings, local businesses, product prices, competitor ads, funding rounds, building permits) in a spreadsheet or an AI agent, without logging in anywhere or copying pages by hand.

**How:** pick a tool below, give it a search, and download the results as CSV, Excel or JSON, or send them to Google Sheets, n8n, Make or an AI agent through the Apify MCP server. Each tool has a runnable Python example repository:

```bash
git clone https://github.com/Aurelix-Solutions/linkedin-jobs-example
cd linkedin-jobs-example && pip install -r requirements.txt
export APIFY_TOKEN=your_token_here && python main.py
```

**Tools site:** every public tool has a page with its live price, example input and output, and an FAQ at [aurelix-solutions.github.io/tools](https://aurelix-solutions.github.io/tools/), plus [step-by-step guides](https://aurelix-solutions.github.io/tools/guides/).

**Price:** pay per result, listed on each tool's Store page, with nothing billed for platform usage on top. Apify's free plan includes $5 of credit a month.

### What to expect from every tool

- **Tested before release.** Each tool passes an independent check: records compared field by field against the source, edge cases, and a privacy scan.
- **Pay only for results.** Clear per-result pricing, no charge for duplicates or empty searches, and lower prices on paid Apify plans.
- **No login, ever.** Tools read only public pages any logged-out visitor can see, at a polite pace.
- **Privacy built in.** Business data and business contacts are kept, private individuals' details are removed, and removal requests are honoured.
- **Maintained daily.** Automatic health checks catch site changes early, and issues get a reply within one business day.

### Tools by use case

Each line says why the tool beats the leading alternatives on the Apify Store, from the comparison table on its Store page.

**Jobs and hiring**

- [LinkedIn Jobs Scraper](https://apify.com/aurelix/linkedin-jobs) - LinkedIn job postings by keyword, country and date posted, with no login: title, company, location, salary where shown, seniority and description. Why this one: exact country filter and filtered-out jobs free; 25% under the most-used LinkedIn scraper on the free plan. [Example](https://github.com/Aurelix-Solutions/linkedin-jobs-example)
- [Greenhouse Jobs Scraper](https://apify.com/aurelix/greenhouse-jobs-scraper) - Jobs straight from company career sites on Greenhouse, Lever, Ashby and SmartRecruiters, in one schema with salary, remote flag and apply link. Why this one: 8x cheaper than the leading jobs API and 40% under the leading feed, read live from each employer's board. [Example](https://github.com/Aurelix-Solutions/career-site-jobs-example)
- [Multi Job Board Scraper](https://apify.com/aurelix/multi-job-board-scraper) - One job search across LinkedIn, company career sites and remote boards, with duplicates merged into one schema. Why this one: LinkedIn plus ~50 company career sites in one deduplicated search, 25% under the alternatives. [Example](https://github.com/Aurelix-Solutions/multi-board-jobs-example)

**E-commerce and product research**

- [Amazon Best Sellers Scraper](https://apify.com/aurelix/amazon-best-sellers) - Amazon Best Sellers and New Releases by category in 10 marketplaces: rank, ASIN, price, rating and reviews, plus rank changes since your last run. Why this one: 69% under the most-used Best Sellers scraper ($1.80 vs $5.90 per 1,000), 10 marketplaces incl. amazon.ca. [Example](https://github.com/Aurelix-Solutions/amazon-best-sellers-example)
- [AliExpress Scraper](https://apify.com/aurelix/aliexpress-product-search) - AliExpress search results for any keyword: price, original price, discount, rating, units sold and ship-from country. Why this one: cheapest of the three we compared ($1.80 vs $2.49-$9.00 per 1,000), sponsored results flagged. [Example](https://github.com/Aurelix-Solutions/aliexpress-product-search-example)

**Leads and local business**

- [Google Maps Business Scraper](https://apify.com/aurelix/google-maps-scraper) - Google Maps business listings by keyword and city: categories, address, phone, website, rating, hours and coordinates. No review text. Why this one: $1.50 per 1,000 places, less than half the leading Google Maps scrapers ($4-5), with many cities per run and an only-new-places mode. [Example](https://github.com/Aurelix-Solutions/google-maps-businesses-example)
- [Recently Funded Companies](https://apify.com/aurelix/recently-funded-companies) - US companies that just raised a private round, from official SEC Form D filings: offering size, amount sold, industry, executives and directors, plus an optional website and contacts. Why this one: funds and SPVs removed by default, a free only-new-filings mode and the company website confirmed against the filing, which the Form D alternatives compared do not offer. [Example](https://github.com/Aurelix-Solutions/recently-funded-companies-example)
- [Funded Companies Hiring](https://apify.com/aurelix/funded-companies-hiring) - US companies that just raised money (new SEC Form D) joined to their confirmed website, every open role on their own job board and the business contacts they publish, as a monitor that alerts only on new raises and new roles. Why this one: $20 per 1,000 hiring companies against $30 for the other Form D plus jobs Actor, seven job-board systems including Workday instead of three, and company contacts charged only when found. [Example](https://github.com/Aurelix-Solutions/funded-companies-hiring-example)

**Ad research**

- [Facebook Ad Library Scraper](https://apify.com/aurelix/facebook-ad-library-scraper) - Business ads from the public Meta Ad Library by keyword, page ID or Ad Library URL: ad text, media links, dates and platforms. Political ads excluded. Why this one: $0.70 per 1,000 ads vs $5.80 for Apify's own Facebook Ads Scraper, with exact limits and a new-ads-only mode. [Example](https://github.com/Aurelix-Solutions/facebook-ad-library-example)

**Public records**

- [Canada Building Permits Scraper](https://apify.com/aurelix/canada-building-permits-scraper) - Development applications and building permits from seven Canadian cities' open data: address, ward, type, status and value. No owner names. Why this one: the only one with development applications and a ward filter, and the cheapest of the three ($3.00 vs $3.50-$5.00). [Example](https://github.com/Aurelix-Solutions/canada-development-applications-example)

**Web and AI**

- [Website to Markdown Crawler](https://apify.com/aurelix/website-to-markdown) - Each page of a website as clean Markdown of its main content for AI, RAG and LLMs, with title, headings and links. Why this one: a flat $1.50 per 1,000 pages, 34% under Apify's RAG Web Browser and no compute-unit billing; failed pages free. [Example](https://github.com/Aurelix-Solutions/website-to-markdown-example)

**Marketing and SEO research**

- [Google Trends Scraper](https://apify.com/aurelix/google-trends-scraper) - Google Trends for any number of keywords on one 0-100 scale: interest over time, interest by country, state, metro or city, and top and rising related queries. Why this one: $1.50 per 1,000 results vs $3.00 plus platform usage for Apify's own Google Trends Scraper, and it accepts Google Trends explore links. [Example](https://github.com/Aurelix-Solutions/google-trends-example)

### Example code

Each tool has a small public example repo, `Aurelix-Solutions/<tool>-example`, with a runnable Python script (apify-client) that starts the tool, prints a few fields and saves a CSV, plus notes on Google Sheets and n8n. The code is MIT licensed. [awesome-aurelix](https://github.com/Aurelix-Solutions/awesome-aurelix) lists them all.

### Need something?

Open an issue on any tool's **Issues** tab on the Apify Store for bugs, feature requests or a custom data source. Feedback and reviews help us decide what to build next.

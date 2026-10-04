# Arcturus Crawler

Arcturus is a public-source monitoring crawler used by **Actually A Deal**.

It is designed to collect limited public evidence from explicitly approved sources so that emerging consumer buying intent can be identified and reviewed.

## What Arcturus does

Arcturus may access approved public sources such as:

- public RSS or Atom feeds
- documented public APIs
- other explicitly approved public pages or endpoints

Collection is intentionally conservative and limited to the evidence needed for analysis and provenance.

## What Arcturus does not do

Arcturus does not:

- bypass authentication
- bypass paywalls
- bypass CAPTCHAs
- evade technical access controls
- rotate identities to avoid blocking
- impersonate normal users or browsers deceptively
- access private or account-only content without authorisation
- ignore robots.txt
- continue collecting from a source after an applicable opt-out or suppression decision

Technical accessibility is not treated as permission.

## Crawler behaviour

Arcturus uses a stable crawler identity and conservative request rates.

Where applicable it uses:

- robots.txt checks
- low-frequency polling
- caching
- change detection
- duplicate suppression
- bounded response sizes
- bounded evidence excerpts
- backoff after rate limits, access denials, server errors or network failures

Arcturus is not intended to perform broad or aggressive web crawling.

## Purpose

The purpose of Arcturus is to identify public evidence of consumer demand and buying situations for internal analysis by Actually A Deal.

Observed evidence is kept separate from later interpretation, commercial decisions and publishing decisions.

Arcturus does not automatically treat:

- retailer activity as consumer demand
- social attention as purchase intent
- technical availability as permission to collect

## Robots.txt

Arcturus respects robots.txt according to its approved crawler policy.

If a source explicitly disallows collection applicable to Arcturus, the crawler will not attempt to bypass that restriction.

## Opt-out and suppression

Site owners may request that Arcturus stop collecting from their site or feed.

Approved opt-out requests are applied prospectively to future collection.

To request suppression, please contact:

** 1n722h@gmail.com **

Please include:

- the domain or feed URL
- your relationship to the site
- the nature of the request

## Contact

For questions about Arcturus, crawler behaviour, or source suppression:

** 1n722h@gmail.com **

## User-Agent

The crawler identifies itself as:

```text
Bootes-Arcturus/0.1 (+https://1n722h.github.io/arcturus-crawler-info/)

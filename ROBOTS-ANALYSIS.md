# Robots Analysis for the Daily Pennsylvanian

The Daily Pennsylvanian's `robots.txt` file is available at
[https://www.thedp.com/robots.txt](https://www.thedp.com/robots.txt).

## Contents of the `robots.txt` file on [2/24/25]

```
User-agent: *
Crawl-delay: 10
Allow: /

User-agent: SemrushBot
Disallow: /
```

## Explanation

1. User-agent: *
	•	This applies to all web crawlers (denoted by *).

2. Crawl-delay: 10
	•	This instructs crawlers to wait 10 seconds between successive requests to the website.
	•	Helps reduce server load and prevent excessive requests from overwhelming the website.

3. Allow: /
	•	Allows all crawlers to access all pages of the website (/ means the root directory and everything under it).

4. User-agent: SemrushBot
	•	This targets a specific bot called SemrushBot (which is used for SEO and competitive analysis).

5. Disallow: /
	•	This blocks SemrushBot from crawling any part of the website.

# Explanation of Changes to script.py

I chose to change the scraper to scrape the headline from the top article of the Multimedia page. I did so by changing the request URL from https://www.thedp.com to https://www.thedp.com/multimedia so that the scraper directly accessed the multimedia page. Then, using inspect element, I found that the class of the top headline was "medium-link" so I changed the target element class to "medium-link"- thus collecting the top headline from the multimedia page.

# Explanation of Cron Schedule Change

The initial cron expression 0 20 * * * meant that my job runs at 8:00 PM UTC every day. The five fields in this expression are minute, hour, day of month, month, and day of week, and I found that you are able to have multiple times by inputting two parameters separated by a comma for one of the fields. I wanted my scraper to run once at 8:00 AM UTC and again at 8:00 PM UTC for a total of two runs per day. Thus, I changed the cron expression to reflect this by modifying it to "0 8,20 * * *", where the 8,20 replaces 20 marking the change from running once at 8:00 PM to running twice at 8:00 AM UTC and 8:00 PM UTC.

# Web Scraping
[How to web scrape with Python](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)

I've actually done a decent bit of this before the class. Using beautiful soup to pull NASAs image of the day.

```from bs4 import BeautifulSoup```

> one_a_tag = soup.findAll(‘a’)[38]  
link = one_a_tag[‘href’]

>This code saves the first text file, ‘data/nyct/turnstile/turnstile_180922.txt’ to our variable link. The full url to download the data is actually ‘http://web.mta.info/developers**/**data/nyct/turnstile/turnstile_180922.txt’ which I discovered by clicking on the first data file on the website as a test. We can use our urllib.request library to download this file path to our computer. We provide request.urlretrieve with two parameters: file url and the filename. For my files, I named them “turnstile_180922.txt”, “turnstile_180901”, etc.

> download_url = 'http://web.mta.info/developers/'+ link  
urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:])

# [Scraping without getting blocked](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)

### This is the good stuff here.

Most websites will automatically detect and block addresses that are scraping data. 
While scraping data isnt Illegal, its a little bit of a grey area. And many companies dont allow their data to be scraped. 

A simple crawler that is scraping a website can easily overload a low power hosting server.

Here are a few easy giveaways that you are bot/scraper/crawler –

-   Scraping too fast and too many pages, faster than a human ever can
-   Following the same pattern while crawling. For example – go through all pages of search results, and go to each result only after grabbing links to them. No human ever does that.
-   Too many requests from the same IP address in a very short time
-   Not identifying as a popular browser. You can do this by specifying a ‘User-Agent’.
-   using a user agent string of a very old browser

It can help to disquise your scraping if you build it some random clicks/ or rest periods into your scraper. essentially making it look human. 
# Read: Class 17 Web Scraping

## Web Scrape with Python in 4 minutes
- Web scraping is a technique to automatically access and extract large amounts of information from a website.
- Read terms and conditions of the website so you know exactly how to use the data.
- You may get blocked from the site if you download data at too rapid a rate because it may break the website.
- Use inspect on a web page then click on the arrow symbol and select the thing on the website,
	it will show you the raw code of that item.	

- After getting the url of the website and creating a new variable like:
	url = '<websit url>'
	response = requests.get(url)
	- After that we use soup = BeautifulSoup(response.text, "html.parser")
	- Beautiful Soup is a library that it makes a nicer data structure.
- Can use soup.findAll('a') and it will give us the result of all 'a' tags of the website

- You  should always use time.sleep(1) to pause your code for a second so that you stop spamming the website
	with requests. This line of code actually helps avoiding getting flagged from the website as a spammer.
- Supervised machine learning model is when a model learns from data that is already labeled.


## What is Web Scraping?
- Web scraping is also called web data extraction or web harvesting which is used for extracting data form websites.
- Web scraping software may directly access the world wide web using Hypertext Transefer Protocol or web browser.
	while web scraping can be done manually by a software user.
- Fetching is downloading of a page(which the browser does when a user views a page).
- Web crawling is  a main component of web scraping to fetch pages for later processing.
- JSON is commonly used as a transport storage mechanism between the client and the web server.
	- [Click for soruce](https://en.wikipedia.org/wiki/Web_scraping)
- API stands for **Application Programming Interface** which is an interface that makes it easier to develop
 	a program by providing the building blocks.

1. The simplest form of web scraping is copying and pasting data form a web page into a text file or spreadsheet.
2. Text Pattern Matching:
	- A simple yet powerful approach to extract information from web pages can be based on the UNIX grep command or
		 regular expression-matching facilities of programming languages (for instance Perl or Python).
3. Static and dynamic web pages can be retrieved by posting HTTP requests to the remote web server using socket programming.
4. HTML Parsing.
5. DOM Parsing.
6. Vertical Aggregation.
7. Semantic annotation recognizing.
8. Computer vision web page analysis.


## How to scrape websites without getting blocked
- First tip is to set a sleep time so you don't spam the website with too many requests
- There are tools that makes sure that you are a human or a bot and they know that because human beings are random
	and bots aren't. they can tell by:
	1. Scraping too fast and too many pages, faster than a human ever can
	2. Following the same pattern while crawling
	3. Too many requests from the same IP address in a very short time
	4. Not identifying as a popular browser. You can do this by specifying a ‘User-Agent’.
	5. Using a user agent string of a very old browser.
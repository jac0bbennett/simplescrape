# simplescrape.py

This is a simple and extremely lightweight web page scraper especially designed for articles. The scraper retrieves the page's title, description, meta image, and favicon if present. The module uses techniques found in testing to find the favicon almost everytime.

## Usage
```python
import simplescrape

url = 'http://www.theverge.com/2016/4/12/11416122/there-will-be-a-bot-for-everything'

if simplescrape.check_link(url):
  page = simplescrape.scrape_link(url)
  title = page.title
  description = page.description
  image = page.image
  favicon = page.favicon
```

## Requirements
requests, lxml

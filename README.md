# Actor - Ultimate Proxy Scraper

## Ultimate Proxy Scraper

Ultimate Proxy Scraper is the number one solution to retrieve thousands of free proxies on a second.

The Ultimate Proxy Scraper scrapes over 30+ different data sources and collects all kinds of different Free and Premium proxies for HTTP, HTTPS, SOCKS4 and SOCKS5 that you can use.

## Bugs, fixes, updates and changelog

This scraper is under active development. If you have any feature requests you can create an issue from [here](https://github.com/tugkan/ultimate-proxy-scraper/issues).


## Input Parameters

The input of this scraper should be JSON containing the list of pages on Ultimate Proxy Scraper that should be visited. Required fields are:

| Field                | Type    | Description                                                                                                                                                                                                    |
| -------------------- | ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| maxItems             | Integer | (optional) You can limit scraped products. This should be useful when you search through the big subcategories.                                                                                                |
| proxy                | Object  | Proxy configuration                                                                                                                                                                                            |

This solution requires the use of **Proxy servers**, either your own proxy servers or you can use [Apify Proxy](https://www.apify.com/docs/proxy).


### Compute Unit Consumption

The actor optimized to run blazing fast and scrape many as proxies as possible. If actor doesn't block very often it'll scrape 10000 listings in 3 minutes with ~0.09-0.1 compute units.

### Ultimate Proxy Scraper Scraper Input example

```json
{
  "maxItems":500,
  "proxy":{
    "useApifyProxy":true
  }
}
```

## During the Run

During the run, the actor will output messages letting you know what is going on. Each message always contains a short label specifying which page from the provided list is currently specified.
When items are loaded from the page, you should see a message about this event with a loaded item count and total item count for each page.

If you provide incorrect input to the actor, it will immediately stop with failure state and output an explanation of what is wrong.

## Ultimate Proxy Scraper Export

During the run, the actor stores results into a dataset. Each item is a separate item in the dataset.

You can manage the results in any languague (Python, PHP, Node JS/NPM). See the FAQ or <a href="https://www.apify.com/docs/api" target="blank">our API reference</a> to learn more about getting results from this Ultimate Proxy Scraper actor.

## Scraped Ultimate Proxy Scraper Properties

The structure of each item in Ultimate Proxy Scraper looks like this:

### Item Detail

```json
{
  "host": "204.10.182.34",
  "port": "39593",
  "full": "204.10.182.34:39593",
  "type": "SOCKS4"
}
```

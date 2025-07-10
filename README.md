# Amazon Phone Scraping Project

## Table of Contents:

* Objective
* Motivation
* How Does It Work?
* HTML (Optional)
* Web Scraping Workflow
* Ethics of Scraping
* References
* Feedback

---

## Objective

This project shows how to scrape product details for mobile phones from Amazon using Python. We use Selenium and BeautifulSoup to automate browsing and extract information like product title, price, brand, RAM, processor, and more. The final output is saved in a structured CSV file.

## Motivation

Web scraping helps collect large volumes of data from websites. It's especially useful for data analysts and developers who want to gather product listings, pricing trends, or specifications automatically instead of manual copy-pasting.

## How Does It Work?

We use Python libraries like:

* **Selenium**: Automates browser actions like clicking, scrolling, and loading dynamic content.
* **BeautifulSoup**: Parses HTML to extract useful information.
* **Pandas**: Organizes data into structured format (CSV).

We visit multiple Amazon pages, extract product links, visit each product page, and collect detailed data.

## HTML (Optional)

Every website is made of HTML. Understanding tags like `<div>`, `<span>`, `<a>` helps identify where information is located. For example:

```html
<span class="a-size-base a-text-bold">Brand</span>
<span class="a-size-base po-break-word">Samsung</span>
```

The first span is a label and the second span is the value.

## Web Scraping Workflow

1. **Open Browser** using Selenium
2. **Go to listing page** and collect product URLs
3. **Click each product link**
4. **Extract details** using BeautifulSoup
5. **Save data** to CSV using Pandas

This method is scalable, and the code can scrape data across many pages.

## Ethics of Scraping

* Check the site's `robots.txt` file to follow their rules
* Avoid sending too many requests too fast
* Don’t scrape sensitive or copyrighted data
* Use APIs if available
* Add delays between requests to reduce server load

## References

* \[Amazon Product Page HTML structure]
* [BeautifulSoup documentation](https://www.crummy.com/software/BeautifulSoup/)
* [Selenium documentation](https://www.selenium.dev/documentation/)
* [robots.txt documentation](https://www.robotstxt.org/)

## Feedback

If you have suggestions or feedback to improve this project, feel free to reach out or submit an issue in the GitHub repository. We appreciate collaboration!

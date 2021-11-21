# class_17
### Web Scraping
Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort.
#### Inspecting the Website
The first thing that we need to do is to figure out where we can locate the links to the files we want to download inside the multiple levels of HTML tags.
#### Python Code
library : 
* import requests
* import urllib.request
* import time
* from bs4 import BeautifulSoup

<img src='https://www.kdnuggets.com/wp-content/uploads/webscraping-code.jpg'/>

Last but not least, we should include this line of code so that we can pause our code for a second so that we are not spamming the website with requests. This helps us avoid getting flagged as a spammer.
**time.sleep(1)**

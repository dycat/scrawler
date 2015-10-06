# encoding: utf-8
import requests
from bs4 import BeautifulSoup

n=0
url = "http://zznews.gov.cn/news/xinwen/zzsz/"
page = requests.get(url)
soup = BeautifulSoup(page.content, "html.parser")
list = soup.find_all("li", {"class": "item"})
for link in list:
    n=n+1
    print n,link.a["title"]
    print link.span.text
    print link.a["href"]

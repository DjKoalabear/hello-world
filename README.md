
```python

import requests
from bs4 import BeautifulSoup


#make a request to the website  and get the content
urls = ('https://www.cnn.com/' , 'https://www.foxnews.com/' , 'https://www.msnbc.com')
responses = [requests.get(url) for url in urls]

# use the 'html.parser' to parse the page
soups = [BeautifulSoup(response.text, 'html.parser') for responses in responses]

# find the data to extract

data = [soup.find_all(text=['Trump Trial', 'Trump' , 'Israel Attacked']) for soup in soups]

#extract and print all data it finds

for data_item in data:
    for item in data_item:
        print(item.get_text())

```
```python

```
```python
# hello-world
my first repository to practice flow and other things
I've always been facinated by tech. It's weird that I didn't get it until now though. Like reallllllly get it. It's cool to understand things and actually get solution out of the problem and that solution be correct. That has always been a bit hard for some reason.

Going to attempt to create a new branch and then merge it back to the master branch. I think that's the flow. I'm not sure. I'll find out soon enough. 
```
Definitely not the best README.md file but it's a start. I'll get better at this. 
```
# This is a new line that I added to the README.md file. 
```
I'm going to add a new line to the README.md file. 
```
def() {
  console.log('Hello World');
}
```
Sick. Lets add another line

My name is Ivan Kowalczyk

Adding another line to the README.md file. 
```
Def() {
  console.log('Ivan Kowalczyk');
}
`
Okay very cool. Now i want to create a database and then connect to it. 
```python
import sqlite3
Cool
``` 
alright lets create a web scraper

```python
pip install beautifulsoup4

#make a request to the website  and get the content
r=requests.get('https://www.google.com')
r.content

# use the 'html.parser' to parse the page

soup = BeautifulSoup(r.content, 'html.parser')

# find the data to extract

data = soup.find_all('quantum physics research', class_= 'example')

#extract and print all data it finds

for item in data:
  print(item)
```
```python

```
```python

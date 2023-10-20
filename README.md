# Welcome to My First Scraper

## Task
Problem: The problem is to scrape the top 25 trending repositories from Github.

Challenge: The challenge is to successfully retrieve, parse, and format the data in a CSV format.


## Description
Solution: I have solved the problem by dividing the task into four parts:

### Part 0: Request
I have created a function request_github_trending(url) that makes a request to the given URL using the requests library in Python and returns the HTML content of the page.

### Part 1: Extract
I have implemented a function extract(page) that uses BeautifulSoup to find all instances of HTML code representing repository rows on the page. This function returns a list of these HTML elements.

### Part 2: Transform
I have created a function transform(html_repos) that takes an array of HTML elements representing repository rows. For each row, it extracts the developer's name, repository name, and the number of stars. It returns this data as an array of hashes, where each hash has the format: {'developer': NAME, 'repository_name': REPOS_NAME, 'nbr_stars': NBR_STARS}.

### Part 3: Format
I have implemented a function format(repositories_data) that takes the array of repository data and formats it into a CSV string. Each column is separated by a comma, and each line by a newline character. The columns in the CSV are: Developer, Repository Name, Number of Stars.




## Installation
To use this project, you need to install the required Python libraries. You can install them using the following commands:

```pip install requests```

```pip install beautifulsoup4```




## Usage
To scrape the top 25 trending repositories from Github, you can run the following command in your terminal:
```python my_scraper.py```

Replace my_scraper.py with the name of your Python script that contains the functions request_github_trending, extract, transform, and format. The script will make the request, extract the data, transform it, and then format it into a CSV string, which you can use as needed.

### The Core Team


<span><i>Made at <a href='https://qwasar.io'>Qwasar SV -- Software Engineering School</a></i></span>
<span><img alt='Qwasar SV -- Software Engineering School's Logo' src='https://storage.googleapis.com/qwasar-public/qwasar-logo_50x50.png' width='20px'></span>

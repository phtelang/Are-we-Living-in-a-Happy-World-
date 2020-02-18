## Are we Living in a Happy World?
In this project, I used BeautifulSoup python package to read and analyze the daily world news from the __[BBC News website](https://www.bbc.com/news/world)__. Using the news URL, I read the entire news article and analyzed word frequencies and assigned sentiment to the news. I created an SQLite database to store world news everyday by date and analyzed the overall news by reading all data from the SQLite database table.

I followed the below steps:
1. Read the news and their urls by web scrapping from the website and add it to a dataframe.
2. Using the url, read each news article and add it to the dataframe.
3. Add sentiment (Positive, Negative, Neutral) to the news article to the dataframe.
4. Add today's news to the database table.
5. Split article sentences into words and get the count for each word.
6. Save top five frequent words in a table in a database for future analysis.
7. Look at the overall news sentiment and day-wise popular words.

### Summary of Results
1. Majority of the news are negative, it does not look like we are living in a happy world.
2. Popular words like said, Trump, told, people, president, government, country appear frequently in the news.
3. Majority of the news are from US and Canada.
4. "said" has been the most popular word consistently.

To view the code and graphs accurately, please __[click on this link](https://nbviewer.jupyter.org/github/phtelang/Are-we-Living-in-a-Happy-World-/blob/master/Are%20we%20Living%20in%20a%20Happy%20World.ipynb)__ as some of the Plotly graphs are not displayed directly on Github.

### Installation
Download the .ipynb (Jupyter file).
Install the requirements using pip install -r requirements.txt. (Make sure you use Python 3.)

### Running the notebook on your machine
An SQLite database will be created in the folder where you placed the .ipynb file. If you want to change the location or of it fails to create the database, you can give an exact file location where you want to place the file.

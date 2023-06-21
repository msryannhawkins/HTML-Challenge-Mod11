# HTML-Challenge-Mod11

In the first part of this challenge, I was tasked with scraping titles and previewing text from Mars News
To begin, I opened the Jupyter Notebook in the starter code folder named part_1_mars_news.ipynb. I worked in this code as I followed the steps below to scrape the Mars News website.

I used automated browsing to visit the Mars news siteLinks to an external site. I inspected the page to identify which elements to scrape. In order to do this, I createed a Beautiful Soup object and used it to extract text elements from the website.After I extracted the titles and previewed text of the news articles that I scraped, I stored the scraping results in Python data structures as follows:

    *I stored each title-and-preview pair in a Python dictionary and, gave each dictionary two keys: title and preview. An example is the following:
            {'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
             'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
    *I then stored all the dictionaries in a Python list.

    *I printed the generated list in my notebook and stored the scraped data in a file (to ease sharing the data with others). To do so, I exported the scraped data to a JSON file.

For Part 2, I was asked to scrape and analyze Mars Weather Data.
To do this, I again used the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb. I worked in this code as I followed the steps below to scrape and analyze Mars weather data.

Like before in Part 1, I used automated browsing to visit the Mars Temperature Data SiteLinks to an external site. I inspected the page to identify which elements to scrape. Note that the URL was https://static.bc-edx.com/data/web/mars_facts/temperature.html.

Again, I created a Beautiful Soup object and used it to scrape the data in the HTML table. I noted that this could also be achieved by using the Pandas read_html function. However, I used Beautiful Soup here to continue sharpening my web scraping skills.

I then assembled the scraped data into a Pandas DataFrame. I ensured that the columns should have the same headings as the table on the website. Then I analyzed my dataset by using Pandas functions to answer the following questions:

            -How many months exist on Mars?
            -How many Martian (and not Earth) days worth of data exist in the scraped dataset?
            -What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question, I used the average minimum daily temperature for all of the months. I then plotted the results as a bar chart.
            -Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question, I found the average daily atmospheric pressure of all the months. Again, I plotted the results as a bar chart.
            -About how many terrestrial (Earth) days exist in a Martian year? To answer this question, I considered how many days elapse on Earth in the time that Mars circles the Sun once. After calculating this, I visually estimated the result by plotting the daily minimum temperature.
            
Finally, I exported the DataFrame to a CSV file.


************************************************************************
Requirements
Part 1: Scrape Titles and Preview Text from Mars News (40 points)
Automated browsing (with Splinter) was used to visit the Mars news site, and the HTML code was extracted (with Beautiful Soup). (10 points)

The titles and preview text of the news articles were scraped and extracted. (20 points)

The scraped information was stored in the specified Python data structure—specifically, a list of dictionaries. (10 points)



Part 2: Scrape and Analyze Mars Weather Data (60 points)
The HTML table was extracted into a Pandas DataFrame. Either Pandas or Splinter and Beautiful Soup were used to scrape the data. The columns have the correct headings and data types. (15 points)

The data was analyzed to answer the following questions: (10 points)

How many months exist on Mars? (5 points)
How many Martian days' worth of data are there? (5 points)
The data was analyzed to answer the following questions, and a data visualization was created to support each answer: (30 points)

Which month, on average, has the lowest temperature? The highest? (10 points)
Which month, on average, has the lowest atmospheric pressure? The highest? (10 points)
How many terrestrial days exist in a Martian year? A visual estimate within 25% was made. (10 points)
The DataFrame was exported into a CSV file. (5 points)

# Web-Scraping

## Table of Contents

- [Project Overview](project-overview)
- [Data Source](data-source)
- [Tools Used](tools-used)
- [Major steps involved](major-steps-involved)
- [Limitations](limitations)
- [Recommendations and further scope](recommendations-and-further-scope)

### Project Overview

In this project, I've tried to scrape some data from an online website 'daft.ie' which is a popular property listing website in Ireland. Since I was moving to Ireland for my masters, I myself was searching for accommodations on various online property listing websites. This is where I came across this idea of scrapping all the properties on rent in Ireland. In this project I've tried to extract the name and address of the property, all the facilities available, how many times this property has been viewwed, and it's corresponding Daft Id.

### Data Source

All the data has been scrapped from [daft.ie](https://www.daft.ie/)

### Tools Used

1. Jupyter Notebooks for data analysis [Jupyter Notebook](https://jupyter.org/), [Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html)
2. Any standalone code editors like [VS Code](https://code.visualstudio.com/), [PyCharm](https://www.jetbrains.com/pycharm/) with Python environment set-up 
3. Microsoft Excel [download here](https://www.microsoft.com/en-in/microsoft-365/excel)

### Major steps involved

1. Importing all the necessary Python libraries like BeautifulSoup, Pandas, NumPy, and other libraries like requests, json, etc.
2. Defining the source url from where the data is to be scrapped, header information, http requests.
3. Once all the above prerequisites have been defined, we first extract the entire HTML data of the webpage and parse it through html parser.
4. From this HTML data, we can then extract  all the anchor tags and other required tags containing the information that is to be scrapped.
5. After all the data has been identified and extracted, ew can define a dataframe using pandas, and append all the necessary information into the dataframe which can then be imported into a csv file.

### Limitations

The html structure of the daft website is a bit complex which makes it a bit difficult to extract the information as required, like under facilities and statistics all the information couldn't be extracted with commas. So I had to use nested 'find' statements and further clean the data in Excel to make it readable and presentable.

### Recommendations and further scope

- In this project, I've just scrapped listings from the first page as I couldn't find a way to go to the next pages on the website, this can be iterated for the rest of the pages by initializing a loop.
- The data imported in the csv can be cleaned further and used for analysis and visualizations by creating insightful reports.





Happy Scrapping! 😄 💻

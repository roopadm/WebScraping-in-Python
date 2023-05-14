<h1 align="center">
  <a href="https://pll.harvard.edu/catalog" target="_blank">
    <img src="https://github.com/roopadm/WebScraping-in-Python/blob/main/images/Harvard_shield_wreath.svg.png" alt="HarvardU" width="60" height="60" style="vertical-align: middle;"/>
  </a>
  <strong>Web scraping all courses on Harvard University Site for different difficulty levels using Python</strong>
  <a href="https://docs.python.org/3/" target="_blank">
    <img src="https://github.com/roopadm/WebScraping-in-Python/blob/main/images/768px-Python.svg.png" alt="Python" width="50" height="50" style="vertical-align: middle;"/>
  </a>
</h1>

<p align="center"> <img src="https://github.com/roopadm/WebScraping-in-Python/blob/main/images/download.png" alt="Projectimage" width="80%" height="10%"/> </p>


<a href="https://www.geeksforgeeks.org/what-is-web-scraping-and-how-to-use-it/" >Web scraping </a> is the process of automatically extracting and parsing data fom websites using a program or tool.Scraping often involves accessing a website's HTML code, parsing and extracting the required information.Web scarping purposes are not just limited to research, infact they are also widely used in business intelligence, building machine learning applications database and also to monitor website changes.
Though web scarping can also be done manually,but using tool or library are considered more efficient.Popular web scarping tools and libraries are Beautiful Soup,Seleniu,Scrapy and Puppeteer.


<a href="https://pll.harvard.edu/catalog"> Harvard University </a> is a prestigious and well-known university that offers wide range of courses covering variety of subjects such as computer science, public health, history, literature and much more. Many students across the globe with engaging lectues and challenging assignments found Harvard's courses to be of high quality. 
The courses are available to all learners irrespective of their background or experience.

However, it is important to carefully opt for the courses which alligns with our interests, level of knowledge or expertise and learning mode preferences and also goals.

### Problem Statement:

Write a Python function to scrape all course data from multiple pages of the **Harvard University Website** based on different difficulty level of courses. Also, write a function to create three CSV(commo-separated values) files , one for each level of course : Introductory, Intermediate, and Advanced. The output CSV should contain course details : course title, course subject area, course modality, course description, course price, and also course link.

### Result :

<p align="center"> <img src="https://github.com/roopadm/WebScraping-in-Python/blob/main/images/csv_image.PNG" alt="Projectimage" width="80%" height="10%"/> </p>

### Accessing tags :

HTML class tag is an attribute used to group elements based on their common functionality or characteristics.
Our HTML document :

<p align="center"> <img src="https://github.com/roopadm/WebScraping-in-Python/blob/main/tags.png" alt="Projectimage" width="80%" height="10%"/> </p>

In the above example, the 'div' element has a class attribute with a value of "group-right". We can use this class value to select all the elements inside this section using a web scraping library BeautifulSoup. We will use the find_all() method to find all the element with a class of "group-right".

Now, we will find course titles,subject area, mode of learning, course description, and price using their associated elements inside the class section of value "group-right". For Course title: the element has class value of "field field-name-title-qs"

For code check out : [Jupyter Notebook](https://github.com/roopadm/WebScraping-in-Python/blob/main/Harward_University_Courses_Webscrape_Final%20(1).ipynb)


## Summary
The initial code includes import statements for necessary libraries, such as pathlib, pandas, BeautifulSoup, numpy, time, and selenium. These libraries are used for web scraping and data manipulation.

The get_link(course) function extracts the link to the detailed information page of a course. It uses Beautiful Soup to find the appropriate HTML element and retrieves the href attribute.

The course_info(course_doc) function extracts information about courses from a Beautiful Soup object representing a course page. It finds specific HTML elements using Beautiful Soup and retrieves the text content. The course information is stored in a dictionary.

The convert_csv(c) function converts a list of dictionaries containing course information into a CSV file. It uses pandas to create a DataFrame from the list and saves it as a CSV file. The name of the generated file is printed.

The if __name__ == ‘__main__’: block is the main entry point of the script. It executes a series of actions: — Initializes an empty list clist to store course information. — Defines a list of difficulty levels tagList. — Iterates over each difficulty level in tagList and a specific range of pages (in this case, only page 0). — Retrieves the course page for each difficulty level and page number using get_courses_page(). — Extracts course information from the retrieved page using course_info() and appends it to clist. — Iterates over each set of course information in clist and converts it to a DataFrame. — Checks if the CSV file “courses.csv” already exists. — If it exists, appends the Data Frame to the existing file without the header. — If it doesn’t exist, creates a new file with the header.

Overall, the code performs web scraping of course information from Harvard University’s website for different difficulty levels. It extracts course details such as title, subject area, mode, description, price, and link to the detailed information page. The course information is then stored in a CSV file named “courses.csv”.

### Future Work
1. Analyzing the scraped data to gain insights and identify patterns.
2. Visualizing the data using tools like matplotlib, seaborn, or Tableau.
3. Building a recommendation system that suggests courses to users based on their interests.
4. Automating the scraping process to run on a regular schedule and keep the course data up to date.

## Check out my other projects too : :mag: 👨‍💻 🛰️

<code>[Data-Driven Marketing Strategies for Rider Conversion : Rider Usage Analysis with R and Tableau](https://github.com/roopadm/Rider-Usage-analysis-R-Tableau)</code> 📊

<code>[An Analysis of Developer Communities: Insights from the 2022 Stack Overflow global Survey](https://github.com/roopadm/AnalyzingDevSurvey-Data-analysis-using-Python)</code> 📊

<code>[A Deep Dive into Indian Hardware Company's Sales Performance: Profit and Revenue Analysis with SQL and Tableau ](https://github.com/roopadm/Sales-Performance-Analysis-using-SQL-and-Tableau-AtiQ/edit/main/README.md) </code> 📊

<code>[ Data Visualization with Tableau : Identify fake website ](https://github.com/roopadm/Identify-Fake-Website-Tableau-excel/edit/main/README.md) </code> 📊

<code>[ Superstore-Sales-performace-Tableau ](https://github.com/roopadm/Superstore-Sales-performace-Tableau/edit/main/README.md) </code> 📊

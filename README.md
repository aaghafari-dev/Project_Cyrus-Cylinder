## Part 1 – API Data Collection

To retrieve structured data from the Wikipedia REST API and convert it into a Pandas DataFrame.



#### API Used

#### Wikipedia REST API endpoint:

https://en.wikipedia.org/api/rest\_v1/page/summary/Cyrus\_Cylinder



## Project Structure



project\_root/

│

├── Project\_Cyrus Cylinder.ipynb

├── Project\_Cyrus Cylinder\_API.ipynb

├── README.md

│

├── output/

│   └── (web scraping results)

│

└── output\_API/

&nbsp;   └── (API results)



### Methodology

###### 1- Import Required Libraries: requests, pandas, os



###### 2- Make API Request



Sent a GET request using requests.get()



Verified successful response using status code



###### 3- Parse JSON Response



Extracted relevant fields: Title, Description, Summary (Extract),  Language, Page ID, Timestamp



###### 4- Convert to DataFrame



Structured the extracted data into a Pandas DataFrame.



###### 5- Export to CSV



## Part 2 – Web Scraping



#### 1- Objective



To scrape HTML content from the Wikipedia page and extract textual information.



#### 2- Web Page Scraped

&nbsp;	https://en.wikipedia.org/wiki/Cyrus\_Cylinder

#### 3- Methodology

###### 3-1 Import Required Libraries: requests, BeautifulSoup, pandas,  os



###### 3-2 Request HTML Page



Sent GET request to Wikipedia page



Retrieved raw HTML content



###### 3-3 Parse HTML



Used:

BeautifulSoup(html, "html.parser")



###### 3-4 Extract Content



Collected paragraph <p> elements

Cleaned text

Removed empty entries

Structured results



###### 3-5 Save Results



Saved cleaned text inside:

output/

###### 3-6 Output Generated



cyrus\_cylinder\_scraped\_text.txt












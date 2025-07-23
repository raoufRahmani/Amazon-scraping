## Amazon Product Scraper – Simple Explanation

This code is a **basic tool that helps you scrape any product from Amazon**. You just need to choose the product category you want (like smartphones, watches, headphones, etc.).

### How the code works

The program is divided into **two main parts**:

---

### 1. Getting All the Product Page Links

When you search for a product on Amazon (for example: “smartphones”), there are usually several pages: page 1, page 2, page 3, and so on.

The **first part of the code** asks you to paste the **link of page 2** (you will find this at the bottom of the Amazon search page, where page numbers are listed).

Then the code:

* Removes the "2" from the link to get the base URL
* Asks how many pages you want to scrape (for example: 3 or 5)
* Finds all the links to individual product pages
* Prints how many product links it found

---

### 2. Extracting Product Names and Prices

Once we have all the product links, the **second part of the code** goes through each link and collects:

* The name of the product
* The price (for example: 19,99 €)
* The date of the scraping

Then, it asks you to enter a name for the CSV file (like "smartphones\_data"), and all the product info is saved in that file.

---

## Tools Used

This program uses two Python modules:

* `requests`: to connect to the Amazon website
* `BeautifulSoup`: to read and clean the HTML of the webpage, so we can find the product information

---

## Challenges I Faced

The hardest part was not writing the code, but understanding how the HTML of Amazon is structured. Once I figured out how the product info is stored in the HTML, the rest was much easier.

It was also a bit tricky to know where to place the loops in the code, and how to organize which parts should be inside or outside the loops.

---

## How to Use the Code (Step-by-Step)

1. Go to Amazon and search for a product (for example: “smartphones”)
2. Run the **first part of the code**:

   * It will ask you to paste the URL
   * Then it will ask how many pages you want to scrape ( 2 to 7 pages)
   * It will collect links from all those pages
5. Run the **second part of the code**:

   * It will ask you to choose a name for the CSV file
   * Then it will collect product names, prices, and dates
   * Finally, it will save the results in the CSV file you named

---

By the end, you’ll have a CSV file that includes:

* Product titles
* Prices in euros
* The date of scraping

This file can then be used for data analysis, a school project, or anything else.
I've already made two datasets using the code : smartphones.csv and Laptops.csv. 
If you have any questions or problems to use the code, feel free to contact at any time : 
linkedin : https://www.linkedin.com/in/raoufrhm/
E-mail : rahmaniraouf133@gmail.com  
WhatsApp : +33 7 80 82 40 80  

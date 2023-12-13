# BookMobile Analysis
  See more on this project and others on my [portfolio site](gracefulanalytics.com)


## Context

BookMobile is a travelling library and bookstore whose fleet of buses rotates through rural communities. Their primary business goal is to provide access to excellent books while giving lesser-known authors and publishers opportunities to expand their outreach. As a result, BookMobile's fleet travels year-round and rotates its stock annually to ensure regular opportunities for authors and incentivise customers to return. The company has completed it's first successful tour and is now wanting to evaluate its catalogue and business model before restocking the fleet in preparation for its next tour. 


## Objective

This analysis aims to thoroughly examine BookMobile's extensive catalogue, sales, and checkout database, unveiling the factors driving successes and revealing potential challenges. The analysis will scrutinize both the highest and lowest-performing books to discern the various qualities influencing customer preferences. Key attributes, including formats, genres, and prices, will be explored to pinpoint customer buying habits, forming the basis for informed stocking strategies. The investigation includes a comprehensive dissection of sales and checkout rates systems, evaluating their effectiveness, engagement rates, and providing recommendations for refining operational practices. This in-depth understanding will offer detailed insights into customer engagement patterns, guiding the formulation of effective outreach strategies. The primary objective of this analysis is to empower BookMobile with the knowledge necessary to refine its stocking strategy, ensuring alignment with customer preferences and optimizing overall business efficiency.

## Key Questions

1. What attributes distinguish successful and unsuccessful books?
   
     Analyzing a book's diverse features provides a comprehensive understanding of customer preferences, a crucial factor in making informed stocking decisions
   
2. How do sales and checkout rates compare?
   
     Assessing and contrasting these two models reveals customer engagement preferences that serve as a guide for outreach campaigns.
   
3. How do sales rates for various formats compare?
   
     Stocking multiple formats requires significant storage space. Minimizing duplicates optimizes storage and enables the diversification of the catalogue.
   
4. How does a books various attributes (genre, format, author, ratings) contribute to its sales and checkout rates?
   
     By isolating specific qualities and understanding their impact on a book's sales and checkout rates, we can provide more detailed recommendations for stocking decisions.
   
5. How does a book's price impact its sales rate and potential revenue?
    
     Understanding how a book's price influences its marketability and profit potential is essential for refining pricing strategies to maximize both sales and overall profitability.
      

## Data Source

The data for this project was sourced from Tableau for the explicit purpose of this portfolio project. The data is fictional as is the company, BookMobile and it's associated business objectives. 
The data can be found [HERE](https://help.tableau.com/current/pro/desktop/en-us/bookshop_data.htm)

## Limitations 

- The data provided was only for a single year. This heavily restricts the ability to explore seasonality within sales and checkouts. Additionally, there is no information on books that were stocked in previous years preventing the opportunity to look at genres and author popularity over time.
  
- The ratings table doesn't have a date for when a review was made. As a result, it cannot be determined if reviews have an impact on the likelihood of a book being sold or checked out.

- The checkout table uses a book's *book_id* to identify what book was checked out. As this ID includes all formats and prices of that title it is not possible to identify pricing and formatting trends within checkouts.  

## Challanges

Sales vs Checkouts:

Comparing sales and checkout rates posed various challenges, primarily arising from the sales table referencing books by their ISBN, while the checkout table utilized their book_id. The ISBN, unique for each combination of title, format, and price, facilitates straightforward analysis and comparison of these metrics. On the other hand, the book_id, specific to a title and inclusive of all formats and prices, hinders the ability to discern the price or format of a checked-out book. This limitation reduces the depth and clarity of insights that could otherwise be extracted from this aspect of the analysis.

Ratings:

The simplicity of the rating system restricts in-depth analysis. Examining the distribution of different scores reveals a clear trend: books with higher ratings tend to have more reviews. This introduces uncertainty about whether customers are genuinely influenced by a book's rating. Moreover, the absence of associated data with the review or indication of whether the book was sold or checked out presents a considerable challenge in distilling specific insights with certainty. The lack of detailed information makes it challenging to draw conclusive conclusions regarding the impact of ratings on customer behaviour.


## Tools

- Excel
- JupyterLab Notebook
- SQLite


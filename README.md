# GoFundMe

This is an ongoing project to examine what types of GoFundMe projects are successful as well which GoFundMe pages are scams
or undeserving of donations.
GoFundMe does not provide an API for obtaining data from GoFundMe pages; therefore, this project is a web scraper utilizing
selenium and chromedriver to navigate through the GoFundMe website to extract the top GoFundMe urls.
 I then use requests and BeautifulSoup to parse the raw html of each url in a systematic fashion. I can either directly
extract information from the urls using regex and BeautifulSoup, or engineer features for the dataset (such as getting the latitudes and longitudes from the city where the user has created the GoFundMe). 

The dataset can be accessed easily either by downloading raw tab-delimited `GFM_data.csv` or by loading the `clean_GFM_data.RData` file by installing the R package (to include roxygen2 documentation) with the following command:

```{R}
devtools::install_github("lmeninato/GoFundMe")
```
To be added: documentation on the methodology of how the data was scraped. 
# GrilledScraper
# Purpose
This project was developed as a price discovery tool from historical sold prices of various items listed on grailed.com. This project was purposely built to be deployed in Google Colabs cloud based ipython notebook. The code is very flexible and light in design. There are some parts I will work to fix such as the use of the CSV and Pandas library where only one library is needed. Moreover, this application uses a selenium library (kora.selenium) specifically designed for the Google Colab environment. I must thank Korakot Chaovavanich (@korakot) for the selenium library and user:mack on stackoverflow for helping edit the code. 
# Considerations 
Because Grailed.com is written in JSreact (Javascript) all information must be found as a css element not via XPATH or the encoded values will be compiled into a string as a webelement. BeautifulSoup can then parse the html tags, however, this was found to be too cumbersome and difficult to properly convert to an array from the text strings. Additionally, this code can only be run between 10-20 times per session before a hosting error must be resolved by restarting the runtime. To save the CSV in google drive the !CP save file to directory must be a manual input to specify location and file name.
#Update 04/25/2022
As of this date the Kora Selenium package is no longer maintained and is failing. Furthermore, because of security changes at Grailed.com usuers must have an authenticated account before they can view previously sold items. I have plans to revisit this project at a later date.
# Disclaimer 
This project was a proof of concept and is not meant to be used as a commercial tool or used by any company or firm. I do not grant permission for this code to be used for commercial use. 

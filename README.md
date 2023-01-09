# Ambulance Victoria Quarterly Reports PDF Scraper
A script to improve accessibility of AV quarterly response times data.

![image](https://user-images.githubusercontent.com/69304112/203903340-67013849-2260-410f-910a-3711037dfebe.png)

Ambulance Victoria publishes quarterly reports throught the year with various gauges of its response times. 

Unfortunately, these are only available as a PDF. 

Using Fitz, a Python library, it is possible to extract the most important pieces of this data. 

As there are some slight irregularities in the way the data is return, this is not as straightforward as it could be, but this script takes a modular approach to dealing with those disuniformities, in order to collect and collate and return a dataframe.

It also deals with updates that occour in the series by working backwards throught the reports and only looking for data from previous periods that are not already in the dataframe. 

In combination with data from annual reports, and from the Productivity Commission, this data formed the basis of an RMIT ABC Fact Check analysis of a claim made by the Victorian premier several times during the 2022 Victorian election. 


https://www.abc.net.au/news/2022-11-25/fact-check-daniel-andrews-ambulance-response-times/101697400

We found his claim to be spin.

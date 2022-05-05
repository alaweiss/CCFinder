#################################################
## Scrape updated CCFinder data

rm(list = ls())

# Setup
## Libraries
library(tidyverse)
library(tidylog)
library(RSelenium)
library(xml2)

site_test = "https://www.childcarefinder.gov.au/service/335213440"

#############
# shell('docker run -d -p 4445:4444 selenium/standalone-firefox')

# start driver
remDr <- remoteDriver(remoteServerAddr = "localhost", port = 4445L, browserName = "firefox")

# Open browser tab
remDr$open()

remDr$navigate(site_test)
remDr$getTitle()

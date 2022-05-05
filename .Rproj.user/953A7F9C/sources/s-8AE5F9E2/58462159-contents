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

############
# Web scrape test
# shell('docker run -d -p 4445:4444 selenium/standalone-firefox')

## Start driver
remDr <- remoteDriver(remoteServerAddr = "localhost", port = 4445L, browserName = "firefox")

## Open browser tab
remDr$open()

## Navigate to site
remDr$navigate(site_test)

## Extract information from site
remDr$getTitle()

## Close browser
remDr$close()

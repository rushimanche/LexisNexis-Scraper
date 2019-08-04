# Lexis Nexis Scraper


## Description

This repository contains a python package for the automated scraping of the Lexis Nexis web service. 

Why use this package/code? There are a small collection of alternative options available however these codesets are either outdated, inefficient, require access to the official API, or are not suitably customisable. These reasons led to the development of this package.  

Whilst our best efforts have been made to ensure that the package is robust, as with any web scraping tasks connection drop outs, delays in obtaining pages may cause issues. Likewise, if the website structure changes we endeavour to do our best to update the package as soon as an issue is raised. 

> **_DISCLAIMER:_** This code was developed for academic purposes. Using this software package may be a violation of the terms of use set out by LexisNexis. By downloading and using this package you do so at your own legal risk.

## Requirements

- Lexis Nexis Subscription (API Access Not Required)
- Python 3
- Chrome Driver
  - Used to simulate a real web browser.
  - Available to download at: https://chromedriver.chromium.org/downloads
- Access to MySQL Database (Optional)

## Installation

### Using PIP

``` pip install lnscraper ```

### Manual Installation

## Usage

### Credentials File

### Storage Option

The data can either be saved into either a mySQL database or a pandas dataframe. These need to be setup, as follows, before the webscraping can be initiated. 

#### MySQL (Recommended)

```python
from lnscraper import mysql_version, authentication
```

#### Pandas

```python
from lnscraper import pandas_version, authentication
```

### Authentications Setup

### Search Terms and Sources

### Running the WebScraper


## Citing This Package
Please accredit this package by citing the following in your references. 

```
@phdthesis{hammocks_2019, title={Identifying Weak Signals of Future Change: Detecting and Analysing Trends in Modus Operandi Through Topic Modelling}, author={Hammocks, Daniel}, year={2019}}
```

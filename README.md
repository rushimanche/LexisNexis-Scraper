# Lexis Nexis Web Scraper

## Overview

This repository hosts a Python package that enables automated scraping from the Lexis Nexis web service. 

This package was designed to address the shortcomings of existing options, which are either obsolete, inefficient, require API access, or lack sufficient customization options. Presently, this package is tailored for academic users, but it can easily be modified to accommodate regular and organizational users. 


## Prerequisites

- Lexis Nexis Subscription (API Access Not Necessary)
- Python 3
- Chrome Driver
  - This tool mimics an actual web browser.
  - It can be downloaded from: https://chromedriver.chromium.org/downloads
- MySQL Database Access (Optional)

## How to Install

### Using PIP

``` pip install lnscraper ```

### Manual Installation

## How to Use

### Credential File Setup
The `credentials.json` file serves as a placeholder for your unique login details. It provides a simple and convenient method for storing and using credentials as it can be modified in any text editor. You simply need to replace the placeholder username and password with your academic login information and save the file. 

### Login Automation
This package is designed to automate the academic sign-in process at regular intervals. To enable this feature, you'll need your institution's login link.

1. Visit https://nexis.com to access the Nexis Service.
2. Select the academic sign-in link. 
3. Locate your institution and select “copy link”. 
4. Paste the copied link into the `credentials.json` file in place of the placeholder URL.
5. Save the file. 

The default options will suit most use cases. However, you may need to tweak a few settings to ensure the correct fields are populated for authentication.

### Storage Selection

Data can be stored in either a MySQL database or a pandas dataframe. You will need to set up these options before initiating the web scraping process. 

#### MySQL (Recommended)

```python
from lnscraper import mysql_version, authentication
```

#### Pandas

```python
from lnscraper import pandas_version, authentication
```

### Input Search Terms and Sources

### Launching the WebScraper


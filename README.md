# Fintech-Module-5-Challenge

# Financial Planning with APIs and Simulations

In this Challenge, you’ll create two financial analysis tools by using a single Jupyter notebook:

Part 1: A financial planner for emergencies. The members will be able to use this tool to visualize their current savings. The members can then determine if they have enough reserves for an emergency fund.

Part 2: A financial planner for retirement. This tool will forecast the performance of their retirement portfolio in 30 years. To do this, the tool will make an Alpaca API call via the Alpaca SDK to get historical price data for use in Monte Carlo simulations.

You’ll use the information from the Monte Carlo simulation to answer questions about the portfolio in your Jupyter notebook.

## Technologies

This project leverages Python 3.9.7 ((default, Sep 16 2021, 16:59:28) [MSC v.1916 64 bit (AMD64)] :: Anaconda, Inc. on win32) with the following packages:
 
* [jupyterlab](https://jupyterlab.readthedocs.io/en/stable/user/urls.html#managing-workspaces-ui) - For information about the jupyter lab remote workspace hosted by a local computer.
 
* [os](https://docs.python.org/3/library/os.html) - This module provides a portable way of using operating system dependent functionality.

* [requests](https://pypi.org/project/requests/) - Requests is a simple, yet elegant, HTTP library.. 
Requests allows you to send HTTP/1.1 requests extremely easily. 

* [pandas](https://pypi.org/project/pandas/) - pandas: powerful Python data analysis toolkit. 
pandas is a Python package that provides fast, flexible, and expressive data structures designed to make working with "relational" or "labeled" data both easy and intuitive.

* [dotenv](https://pypi.org/project/python-dotenv/) - Read key-value pairs from a .env file and set them as environment variables. 
Python-dotenv reads key-value pairs from a .env file and can set them as environment variables. It helps in the development of applications following the 12-factor principles.

* [MCForecastTools](https://pypi.org/project/pandas-montecarlo/) - pandas-montecarlo is a lightweight Python library for running simple Monte Carlo Simulations on Pandas Series data.. 

* [matplotlib](https://matplotlib.org/stable/index.html) - Matplotlib 3.5.1 documentation
Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. 
---

## Installation Guide

Before running the application first install the following dependencies.

```python
import os
import requests
import json
import pandas as pd
from dotenv import load_dotenv
import alpaca_trade_api as tradeapi
from MCForecastTools import MCSimulation
%matplotlib inline 
```

---

## Usage

Load private 'keys' generated from Alpaca in order to access data. Review the endpoint URLs for the API calls to Free Crypto API in order to get the current pricing information for both BTC and ETH.

---

## Contributors

Gerald Cortright and Berkeley Fintech support staff
---

## License

MIT License

Copyright (c) [year] [fullname]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

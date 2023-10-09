# Premier League predictions using fifa ratings

This is the code base I created to both collect football data, and then
use this data to train a neural network to predict the outcomes of football
matches based on the fifa ratings of a team's starting 11.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

You'll need:
  * [Python 3.6](https://www.python.org/downloads/release/python-360/)
  * [pip](https://pypi.org/project/pip/)

To install the dependencies,
```
pip install -r requirements.txt`
```

#### Crawlers

The crawlers are all written using Scrapy. For proper usage it would be
beneficial to first know how to use Scrapy.

For a *quick start*, just go to `./fifa_ratings_predictor/crawler` and
use

```
scrapy crawl <spider name> -o <output file>
```
It goes without saying that if you do use these crawlers, please don't
bombard the sites with a stupid amount of requests - *scrape responsibly.*

I have deliberately left all of the data off of the repo because a) it's
not really my data and b) it's not good practice to have data on a repo.

### Installing

To install everything except the crawler you can run

```
pip install .
```

from the top level directory.

You can then import the methods, for example the
simulator,

```
from fifa_ratings_predictor.simulation import SeasonSimulator
```

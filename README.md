# PrizePicks to CSV
A python script to parse the api for [prizepicks.com](https://app.prizepicks.com/) and output current lines as a csv for each category in a given league.

## Local setup
This script is written in Python 3.9 and developed using a pipenv virtual environment. [Check this out](https://realpython.com/pipenv-guide/) for more information on pipenv. For other virtual environment setup, a requirements.txt file is included.

To use locally, clone this repo and follow the usage instructions below.

## Usage
To generate individual csvs of player lines for the various stats in a given league, run `python scripts/scraper.py {{sport}}`, or, if using pipenv, `pipenv run python scripts/scraper.py {{sport}}`, where `{{sport}}` is one of the supported leagues/sports provided by PrizePicks (see below). CSV files will be generated in the `output` folder.

Example:
`python scripts/scraper.py NFL`

Currently supported sports include:
- NFL
- NFL1H
- MLB
- MLBLive
- Soccer
- NBASZN
- PGA
- Tennis
- CFB
- NHLSZN

## Upcoming development
- Additional sports/leagues as they become available
- Ability to supply a second optional argument corresponding to a PrizePicks category (passing yards, touchdowns, total bases, etc) to generate csvs solely for that category

## Affiliations
I have no affiliation with PrizePicks whatsoever. This script was just a way for me to more easily analyze PrizePicks player lines for personal use. 
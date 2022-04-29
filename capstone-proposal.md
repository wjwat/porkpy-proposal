# Capstone Proposal

## Name of Student

William Watkins

## Name of Project

PorkPy

## Project Goal

Allow a user with an account with [Porkbun](https://porkbun.com/) to access and
use their API to manage their domain names from the command-line.

## MVP

* Communicate with Porkbun API
* Accept command line flags to execute different commands
* Modify DNS records using routes provided by Porkbun

## Stretch Goals

* Sanity check commands passed in
* Fully tested & automate testing with GitHub CI
* Accept JSON formatted commands
* Output as JSON
* Automatically built with GitHub action
* Dockerfile
* Well documented

## Tools, Frameworks, Libraries, APIs, etc.

* [Python](https://www.python.org/)
  - Libraries:
    * `json`
    * `requests`
    * One of: `argparse`, `docopt`, `click`
* [Porkbun API](https://porkbun.com/api/json/v3/documentation)
* [Black](https://github.com/psf/black)
* STRETCH: [pytest](https://docs.pytest.org/en/7.1.x/)
* Environment management of some sort
  - [pyenv](https://github.com/pyenv/pyenv)
  - [poetry](https://python-poetry.org/docs/)
  - [virtualenv](https://virtualenv.pypa.io/en/latest/)
* STRETCH: [Docker](https://www.docker.com/)

## Notes to Instructor

N/A
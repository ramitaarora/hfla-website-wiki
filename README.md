
# HackforLA.org Wiki

This repository contains documentation for the Hack for LA website team. The site is live at [https://hackforla.github.io/website-wiki/](https://hackforla.github.io/website-wiki/) and is generated using [MkDocs](https://www.mkdocs.org/) with the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme.

## Installation

### With Docker

The quickest way to run the site is using Docker:

``` bash
docker pull vraer/hfla-website-wiki:latest
docker run -p 8000:8000 vraer/hfla-website-wiki:latest
```

The site will now be running at <http://localhost:8000>.

### With Python virtualenv

Alternatively, you can install locally using Python:

``` python
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt 
mkdocs serve
```

## Support

If you need help or have questions, don't hesitate to reach out to the project maintainers or the Hack for LA community. You can also check the issues in the [hackforla/website](https://github.com/hackforla/website) repository for ongoing discussions and known issues.

# HackforLA.org Wiki

This repository houses the documentation for the Hack for LA website team. The live site is available at [https://hackforla.github.io/website-wiki/](https://hackforla.github.io/website-wiki/). The documentation is built using [MkDocs](https://www.mkdocs.org/) and is styled with the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme.

**Note**: Issues related to this wiki are tracked in the [hackforla/website repository](https://github.com/hackforla/website). For more information on the current state of the wiki, please refer to the [How to Contribute to the Wiki](https://github.com/hackforla/website/wiki/How-to-Contribute-to-the-Wiki) page.

---

## Getting Started

### Clone or Fork the Repository

Clone your fork or the original repository locally:

```bash
git clone https://github.com/YOUR_USERNAME/website-wiki.git
cd website-wiki
```

## Installation

### With Docker

1. **Pull the Docker Image**: To ensure you have the latest Docker image, run:

    ```bash
    docker pull vraer/hfla-website-wiki:latest
    ```
  
2. **Start the Development Server**: To start the development server, run:

    ```bash
    docker run --rm -it -p 8000:8000 -v ${PWD}:/docs vraer/hfla-website-wiki:latest
    ```

Your site will now be accessible at <http://localhost:8000>.

#### Building the Documentation

To build the documentation into a `site` folder, run:

```bash
docker run --rm -it -v ${PWD}:/docs vraer/hfla-website-wiki:latest build
```

### With Python virtualenv

1. **Create a Virtual Environment**:

    ```python
    python3 -m venv venv
    ```

2. **Activate the Virtual Environment**:

    ```bash
    source venv/bin/activate
    ```

3. **Install Required Packages**:

    ```bash
    pip install -r requirements.txt 
    ```

4. **Start the Development Server**:

    ```bash
    mkdocs serve
    ```

5. **Build the Documentation**:

    ```bash
    mkdocs build
    ```

Your site will now be accessible at <http://localhost:8000>.


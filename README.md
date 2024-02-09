# HackforLA.org Wiki

This repository houses the documentation for Hack for LA's website team. The documentation is built using [MkDocs](https://www.mkdocs.org/) and is styled with the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme.

**Note**: Issues related to this wiki are tracked in the [hackforla/website repository](https://github.com/hackforla/website). 

For more information on the current state of the wiki, please refer to the [How to Contribute to the Wiki](https://github.com/hackforla/website/wiki/How-to-Contribute-to-the-Wiki) page.

---

## Getting Started

### Clone or Fork the Repository

```bash
git clone https://github.com/YOUR_USERNAME/website-wiki.git
```

```bash
cd website-wiki
```

## Installation

### With Docker

The easiest way to get your local mkdocs server running and see your changes in real-time is by using Docker Compose.

1. **Start the mkdocs Server**

    To serve your site locally, run:

    ```bash
    docker-compose up
    ```

    This launches the mkdocs server, which serves your documentation site and listens for changes. Your site will automatically update as you make changes to the documentation.

    If you prefer to run the server in the background, use:

    ```bash
    docker-compose up -d
    ```

2. **View Your Site**

    Open a web browser and go to `http://localhost:8000` to see your mkdocs site live.

3. **Stop the Server**

    To stop the server, if running in the foreground, press `Ctrl+C` in your terminal. For detached mode, use:

    ```bash
    docker-compose down
    ```


### With Python virtualenv

**Note for Windows Users Installing Python:**

During the Python installation process, make sure to select the option **"Add Python 3.x to PATH"**. This step will allow you to run Python and pip commands from the Command Prompt.

1. **Create a Virtual Environment**:

    For macOS/Linux:

    ```bash
    python3 -m venv venv
    ```

    For Windows:

    ```cmd
    python -m venv venv
    ```

2. **Activate the Virtual Environment**:

    For macOS/Linux:

    ```bash
    source venv/bin/activate
    ```

    For Windows:

    ```cmd
    .\venv\Scripts\activate
    ```

3. **Install Required Packages**:

    ```bash
    pip install -r requirements.txt
    ```

4. **Start the Development Server**:

    ```bash
    mkdocs serve
    ```

    Your site will now be accessible at <http://localhost:8000>.

5. **Build the Documentation**:

    Building the mkdocs site generates static HTML files. This step is typically reserved for testing custom hooks or preparing the documentation for deployment.

    ```bash
    mkdocs build
    ```

    This compiles your Markdown files into static HTML files, placing them in the `site` directory.


# HackforLA.org Wiki

This repository contains documentation for the Hack for LA website team. The site is live at [https://hackforla.github.io/website-wiki/](https://hackforla.github.io/website-wiki/) and is generated using [MkDocs](https://www.mkdocs.org/) with the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme.

## Prerequisites

- Ensure you have Python3 installed on your machine.
- Windows users: If you are installing Python for the first time, remember to check the box to add Python to PATH during installation.

## Installation and Setup

1. Fork the [hackforla/website-wiki repository](https://github.com/hackforla/website-wiki) on GitHub and/or clone to your local machine:

```bash
git clone https://github.com/<Your-Username>/website-wiki.git
```

2. Move into the cloned directory:

```bash
cd website-wiki
```

3. Choose from one of the following options:

### Option 1: Python with Conda

<details>
<summary><strong>Installation and Setup Instructions</strong></summary>

- Install Conda:
  - macOS: Use [Homebrew](https://brew.sh/) to install Miniconda:
    ```bash
    brew install --cask miniconda
    ```

  - Windows/Linux: Download and install Miniconda from the official website: [Miniconda](https://docs.conda.io/en/latest/miniconda.html).

- Create and Activate a Conda Environment:
  1. Create a new Conda environment:
    ```bash
    conda create --name mkdocs python=3  # You can replace 'mkdocs' with your preferred environment name, and specify python=3.X for a specific Python version.
    ```
  2. Activate the environment:
    ```bash
    conda activate mkdocs
    ```
  3. Install the necessary packages:
    ```bash
    pip install mkdocs mkdocs-material mkdocs-awesome-pages-plugin
    ```
  4. Deactivate the environment when done:
    ```bash
    conda deactivate
    ```
</details>

### Option 2: Python with venv

<details>
<summary><strong>Installation and Setup Instructions</strong></summary>

- Set up a new Python virtual environment:
  ```bash
  python -m venv venv  # 'venv' can be replaced with your custom environment name
  ```

- Activate the environment:
  - macOS/Linux:
    ```bash
    source venv/bin/activate
    ```
  - Windows:
    ```bash
    .\website-wiki-venv\Scripts\activate
    ```

- Install the required packages using pip:
  ```bash
  pip install mkdocs mkdocs-material mkdocs-awesome-pages-plugin
  ```
</details>

## Previewing the Site

To start the local server:

```bash
mkdocs serve
```

Open a web browser and navigate to **`http://127.0.0.1:8000`**


## Additional Notes on Config

- The `mkdocs-material` package serves as the base theme, which includes several other packages. Any additional non-native plugins enabled in the `mkdocs.yml` file under the `plugins` entry may require specific installation instructions. See [Best of MkDocs](https://github.com/pawamoy/best-of-mkdocs) for a list of popular plugins.
- If your updates involve custom hooks, such as Python scripts linked in the `mkdocs.yml` file in the `hooks/` folder, some changes may only be visible after running the `mkdocs build` command manually.

For more details and customization options, refer to the official [mkdocs-material documentation](https://squidfunk.github.io/mkdocs-material/).


## Editing Markdown Files

 Some things to keep in mind when editing Markdown files for the wiki:


### Python Markdown and Extensions

MkDocs uses Python Markdown, a Python implementation of Markdown that supports extensions for additional features. The specific extensions enabled for the site are listed in the `mkdocs.yml` file under the `markdown_extensions` section. Some of these extensions include:

- `admonition`: This extension adds support for admonitions, which are specially marked "blocks" of text that render as sidebars. They're useful for asides or special notes.

- `codehilite`: This extension adds syntax highlighting to code blocks.

- `toc`: This extension generates a table of contents.

- `tables`: This extension adds support for tables.

- `footnotes`: This extension adds support for footnotes.


### YAML Validation Scheme in VSCode

If you're editing files in Visual Studio Code (VSCode), it's recommended to add the YAML validation scheme for better linting and autocompletion. Here's how you can do it:

1. Open VSCode and go to the Extensions view (`Ctrl+Shift+X`).
2. Search for and install the "YAML" extension by Red Hat.
3. After installation, open the settings (`Ctrl+,`).
4. Search for "YAML Schemas" in the settings search bar.
5. Click on "Edit in settings.json".
6. In the settings.json file, add the following:

```json
"yaml.schemas": {
    "https://raw.githubusercontent.com/squidfunk/mkdocs-material/master/schema.json": "mkdocs.yml"
}
```

7. Save the settings.json file.

This will enable the YAML validation scheme specifically for the `mkdocs.yml` file.


### Differences from GitHub Flavored Markdown

While Python Markdown is similar to GitHub Flavored Markdown (GFM), there are some differences to be aware of:

- **Nested Lists**: In Python Markdown, nested lists require four spaces for indentation, while GFM only requires two spaces.
- **URL Auto-linking**: GFM automatically converts URLs into links, while Python Markdown does not.

For a more comprehensive comparison, you can refer to the [Python Markdown documentation](https://python-markdown.github.io/) and the [GitHub Flavored Markdown Spec](https://github.github.com/gfm/).

Remember, when you're editing Markdown files for the documentation site, always preview your changes locally to ensure they render as expected.


### Linking

- **GitHub Flavored Markdown**: Supports wiki-style links, where you can link to other pages using the page's title in double brackets `[[Page Title]]`.
- **MkDocs**: Uses relative linking, where links are relative to the `docs` directory. For example, to link to a file named `example.md` in a subdirectory called `subdir`, you would use `[Link Text](subdir/example.md)`.

For more information on linking in MkDocs, refer to the [official documentation on linking](https://www.mkdocs.org/user-guide/writing-your-docs/#linking-to-pages).


## Support

If you need help or have questions, don't hesitate to reach out to the project maintainers or the Hack for LA community. You can also check the issues in the [hackforla/website](https://github.com/hackforla/website) repository for ongoing discussions and known issues.

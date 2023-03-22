# Documentation

This documentation is generated with the [MkDocs](https://www.mkdocs.org/) static site generator with the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) design theme. See the respective documentation for detailed information of installation and configuration options.

## Initial Installation  

The initial installation of MkDocs included the following files: 
```
    mkdocs.yml	                        # MkDocs configuration file
    docs/
        index.md                        # folder containing documentation source .md files
    .github/
        workflow/
            ci.yml                      # min. installation of Material theme
        ISSUE_TEMPLATE/                 # sample template .md files
    workflow-templates/                 # test files
    LICENSE
    README.md                        
```
Site is live at [https://hackforla.github.io/website-wiki/](https://hackforla.github.io/website-wiki/)

## Deploying Documents
[Documents are deployed](https://www.mkdocs.org/user-guide/deploying-your-docs/) in the appropriate subfolder under the `/docs/` folder. The documents are deployed whenever the `ci.yml` action is run.

# Configuration Options  
Following are descriptions of some of the many configuration options. 
## MkDocs Plugins  
Plugins available for use with MkDocs are too numerous to describe here, but includes this list of [MkDocs Plugins](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Plugins). This is also available as a [Best of MkDocs](https://github.com/pawamoy/best-of-mkdocs) list of 180 open-source project plugins ranked by users.  

## Material Options  
The Material for MkDocs design theme includes multiple configuration and extension options. Unless noted otherwise, all configurations and extensions are set in the `mkdocs.yml` configuration file.  
- Note: Material for MkDocs recommends installation of its [YAML schema validation](https://squidfunk.github.io/mkdocs-material/creating-your-site/#:~:text=Recommended%3A%20configuration%20validation%20and%20auto%2Dcomplete).   

- Note: MkDocs includes a [live preview server](https://squidfunk.github.io/mkdocs-material/creating-your-site/) in Docker for previewing changes as they are made.  
  


### Material design customizations

- [Additional CSS](https://squidfunk.github.io/mkdocs-material/customization/#additional-css) - using a separate style sheet to adjust specific elements  
- [Additional JS](https://squidfunk.github.io/mkdocs-material/customization/#additional-javascript) - integrating other syntax or adding custom logic to the theme
- [Theme extension](https://squidfunk.github.io/mkdocs-material/customization/#extending-the-theme) - an easy way to override parts of Material for MkDocs without forking from git

### Material design advanced configuration options 

- [Changing the colors](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#changing-the-colors)  
- [Changing the fonts](https://squidfunk.github.io/mkdocs-material/setup/changing-the-fonts/#changing-the-fonts)  
- [Changing the language](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#changing-the-language)  
- [Changing the logo and icons](https://squidfunk.github.io/mkdocs-material/setup/changing-the-logo-and-icons/#changing-the-logo-and-icons)  
- [Ensuring data privacy](https://squidfunk.github.io/mkdocs-material/setup/ensuring-data-privacy/#ensuring-data-privacy)  
- [Setting up navigation](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/#setting-up-navigation)  
- [Setting up site search](https://squidfunk.github.io/mkdocs-material/setup/setting-up-site-search/#setting-up-site-search)  
- [Setting up site analytics](https://squidfunk.github.io/mkdocs-material/setup/setting-up-site-analytics/#setting-up-site-analytics)  
- [Setting up social cards](https://squidfunk.github.io/mkdocs-material/setup/setting-up-social-cards/#setting-up-social-cards)  
- [Setting up a blog](https://squidfunk.github.io/mkdocs-material/setup/setting-up-a-blog/#setting-up-a-blog)  
- [Setting up tags](https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/#setting-up-tags)  
- [Setting up versioning](https://squidfunk.github.io/mkdocs-material/setup/setting-up-versioning/#setting-up-versioning)  
- [Setting up the header](https://squidfunk.github.io/mkdocs-material/setup/setting-up-the-header/#setting-up-the-header) 
- [Setting up the footer](https://squidfunk.github.io/mkdocs-material/setup/setting-up-the-footer/#setting-up-the-footer)  
- [Adding a git repository](https://squidfunk.github.io/mkdocs-material/setup/adding-a-git-repository/#adding-a-git-repository)  
- [Adding a comment system](https://squidfunk.github.io/mkdocs-material/setup/adding-a-comment-system/#adding-a-comment-system)  
- [Building an optimized site](https://squidfunk.github.io/mkdocs-material/setup/building-an-optimized-site/#building-an-optimized-site)  
- [Building for offline usage](https://squidfunk.github.io/mkdocs-material/setup/building-for-offline-usage/#building-for-offline-usage)  

### Python Markdown extension options   
There are two recommended Markdown extension packages, [Python Markdown](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown/) and [Python Markdown Extensions](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/), that are supported by Material for MkDocs. The minimal and recommended configurations for extensions are:   
  
- [Minimal configuration](https://squidfunk.github.io/mkdocs-material/setup/extensions/#minimal-configuration) when using Material for the first time
- [Recommended configuration](https://squidfunk.github.io/mkdocs-material/setup/extensions/#recommended-configuration) that enables all Markdown-related features

- Individual listings of Markdown-related config options from the two packages:
  - [Abbreviations](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown/#abbreviations) – ability to add a small tooltip to an element  
  - [Admonition](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown/#admonition) – support for call-outs (aka admonitions) 
  - [Arithmatex](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#arithmatex) – allows rendering of math typesetting via [MathJax](https://www.mathjax.org/)  
  - [Attribute Lists](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown/#attribute-lists) – allows adding HTML attributes and CSS classes  
  - [BetterEm](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#betterem) – improves detection to emphasize text using special characters, i.e. for bold and italic
  - [Caret, Mark & Tilde](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#caret-mark-tilde) – add the ability to highlight text and define sub- and superscripts  
  - [Critic](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#critic) – allows usage of [Critic Markup](https://github.com/CriticMarkup/CriticMarkup-toolkit) to highlight text/ track changes  
  - [Definition Lists](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown/#definition-lists) – allows usage of definition/ description lists `dl` in HTML  
  - [Details](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#details) – ‘supercharges the Admonition extension’ for collapsible call-outs  
  - [Emoji](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#emoji) – inlines bundled and custom emojis and icons 
  - [Footnotes](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown/#footnotes) – allows defining inline footnotes  
  - [Highlight](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#highlight) – support for syntax highlighting of code blocks 
  - [InlineHighlight](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#inlinehilite) – built on top of Highlight for highlighting inline code blocks  
  - [Keys](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#keys) – adds ability to render keyboard keys (e.g. Ctrl + Alt + Del)  
  - [Markdown in HTML](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown/#markdown-in-html) – allows wrapping markdown content with custom elements in HTML  
  - [SmartSymbols](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#smartsymbols) – converts characters into symbols, e.g. fractions, copyright mark, etc.  
  - [Snippets](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#snippets) – add ability to embed content from arbitrary files into a document  
  - [SuperFences](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#superfences) – facilitates creation of flowcharts, sequence diagrams, etc. including [Mermaid.js](https://mermaid-js.github.io/mermaid/) integration 
  - [Tabbed](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#tabbed) - allows usage of content tabs to group related content
  - [Table of Contents](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown/#table-of-contents) – automatically generates a table of contents
  - [Tables](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown/#tables) – adds ability to create tables in Markdown  
  - [Tasklist](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions/#tasklist) – allows usage of [GitHub Flavored Markdown](https://github.github.com/gfm/) inspired tasklists  

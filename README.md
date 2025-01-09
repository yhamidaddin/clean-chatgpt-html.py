### README for `clean-chatgpt-html.py`

```markdown
# clean-chatgpt-html.py

A Python script that cleans saved ChatGPT HTML pages by removing unnecessary elements like external references, scripts, and extraneous HTML. It outputs a stand-alone HTML file that does not rely on any external resources (images, CSS, or JavaScript). The output file can be easily viewed offline.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Dependencies](#dependencies)
- [License](#license)
- [Contact](#contact)

## Overview

The `clean-chatgpt-html.py` script is designed to clean up saved HTML files of ChatGPT outputs by removing unwanted scripts, external references, and tags. The resulting HTML file is simplified, self-contained, and can be viewed offline without dependencies. This is particularly useful for saving and sharing ChatGPT interactions in a clean format, making them portable and easy to read.

## Installation

### Prerequisites

To run this script, you will need the following Python packages:

- `BeautifulSoup` (from `bs4`): A library for parsing HTML content.
- `lxml`: Required for parsing HTML content efficiently (it’s the default parser for BeautifulSoup).

### Step 1: Install Dependencies

You can install the required dependencies using `pip`:

```bash
pip install beautifulsoup4 lxml
```

### Step 2: Download the Script

Clone the repository containing this script or download the Python file directly.

```bash
git clone https://github.com/yourusername/clean-chatgpt-html.git
```

### Step 3: Ensure Python Environment

Make sure you are running this script in an environment where the dependencies are installed (either a virtual environment or globally).

## Usage

To use the script, follow these steps:

1. Run the Python script:
   ```bash
   python clean-chatgpt-html.py
   ```

2. The script will prompt you to enter the full path of the HTML file you want to process.

   ```bash
   Enter the full path of the HTML file to be processed: /path/to/chatgpt_output.html
   ```

3. The script will clean up the HTML file, remove unnecessary content, and create a new file with the suffix `-clean` added to the original file name.

   Example:
   - Input file: `chatgpt_output.html`
   - Output file: `chatgpt_output-clean.html`

4. The cleaned file will be saved in the same directory as the original file.

### Example

```bash
Enter the full path of the HTML file to be processed: /home/user/chatgpt_output.html
File is opened.
Processed HTML has been saved to /home/user/chatgpt_output-clean.html
```

## Features

- **Removes Unnecessary Tags**: Automatically removes `<script>`, `<iframe>`, and unwanted `<div>` or `<button>` elements.
- **Self-contained HTML**: Cleans the page so it doesn't require any external images, CSS, or JavaScript files.
- **Title Injection**: Adds a custom title to the `<head>` section based on the file name.
- **Invert Color Button**: Adds a button to toggle between light and dark modes for better readability.
- **Stand-alone Output**: The output HTML file is fully self-contained and can be opened offline without relying on external resources.

## Dependencies

This script requires the following Python libraries:

- **BeautifulSoup4**: For parsing HTML and making modifications.
- **lxml**: Efficient HTML parser for BeautifulSoup.

Install them via pip:

```bash
pip install beautifulsoup4 lxml
```

## License

This script is licensed under the **MIT License**. Feel free to modify and redistribute it under the terms of the license.

## Contact

For questions, feedback, or suggestions, please reach out to the author:

- **Author**: Yahya Hamidaddin
- **Email**: [yhamidaddin@open-alt.com](mailto:yhamidaddin@open-alt.com)

```

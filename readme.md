<div align="center">
     <a href="https://github.com/gusye1234/gpt-readme/blob/main/readme-zh.md">
       GPT-written readme in chinese
    </a>
	  <br/>
    <br/>
    <a href="https://github.com/gusye1234/gpt-readme">
      <img src="https://img.shields.io/badge/written_by-GPT-green">
    </a>
    <a href="https://github.com/gusye1234/gpt-readme">
      <img src="https://img.shields.io/badge/could_be-Wrong-red">
    </a>
    <a href="https://pypi.org/project/gpt-readme/">
      <img src="https://img.shields.io/pypi/v/gpt-readme.svg">
    </a>
</div>

*This readme generated by command: `gpt-readme --path="./gpt_readme" --demand="gpt-readme is a shell tool that should be used in commandline. Add detailed commandline usage of gpt-readme. Let user know they can install gpt-readme from pip, or from source github repo gusye1234/gpt-readme" --language="english"`*

# gpt-readme

## Introduction
`gpt-readme` is a Python code library for generating README files. It utilizes the OpenAI GPT-3.5 Turbo model to generate README files based on code. The library provides various functionalities including directory and file summaries, code file summaries, and README generation.

## Get Started
To install `gpt-readme`, you can use either of the following methods:

1. Install from PyPI:
   ```
   pip install gpt-readme
   ```

2. Install from source:
   ```
   git clone https://github.com/gusye1234/gpt-readme.git
   cd gpt-readme
   pip install .
   ```

Once installed, you can use the `gpt-readme` command in the command line. Here is an example of the command line usage:

```
gpt-readme --path <path> --exts <extensions> --language <language> --demand <demand> --out <output_file> --cache <cache> --agree
```

- `--path`: The local path of the code repository or file.
- `--exts`: Comma-separated code extensions to consider.
- `--language`: The target language for the README.
- `--demand`: Additional requirements for the README.
- `--out`: The location to save the generated README file.
- `--cache`: Enable or disable caching of code summaries.
- `--agree`: Agree to send code to OpenAI.

Note: The actual usage and available options may vary depending on the specific implementation and requirements.

## Features
- Generate README files based on code using the OpenAI GPT-3.5 Turbo model.
- Summarize directories and their contents.
- Summarize code files.
- Support for multiple code extensions.
- Customizable README language and additional requirements.

## Implementation
The `gpt-readme` code library consists of the following modules and files:

- `gpt_readme/__init__.py`: The initialization file of the `gpt-readme` module. It imports the `main` function from the `main` module and defines the version number, author, and project link.

- `gpt_readme/__main__.py`: The entry file of the code library. It imports the `main` function from the `main` module and calls it when the script is run.

- `gpt_readme/constants.py`: This file defines variables and functions related to the GPT-Readme project, including mappings of file extensions to programming languages and a function to generate the README header.

- `gpt_readme/dir_summary.py`: This file is used to summarize directories and their contents. It utilizes the OpenAI GPT-3.5 Turbo model to generate summaries based on file and module summaries. It provides an overview of the code library and its components.

- `gpt_readme/file_summary.py`: This file provides the functionality to summarize code files. It uses the OpenAI GPT-3.5 Turbo model to generate summaries based on given prompts.

- `gpt_readme/main.py`: This file is a Python script that generates README files based on code using ChatGPT. It accepts command line arguments such as the path to the code repository or file, code extensions, target language for the README, additional requirements, output file location, caching option, and agreement to send code to OpenAI. It utilizes various external modules and internal modules and functions for its implementation.

- `gpt_readme/prompts.py`: This file defines template strings for generating README documents, including system-level prompts and module-level prompts.

- `gpt_readme/utils.py`: This file provides utility functions for setting up the environment, managing cache configuration, hashing content and directories, building prompts and summaries, and more. It utilizes various external modules and internal modules and functions for its implementation.

## Acknowledgement
The `gpt-readme` code library relies on the following third-party libraries:

- `rich.console`: Provides the `Console` class for rich text output.

Special thanks to the authors and contributors of these libraries for their valuable contributions.


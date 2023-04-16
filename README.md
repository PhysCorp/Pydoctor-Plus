# Pydoctor-Plus
### A method of generating documentation using pydoctor and some bash magic for Python projects that are not object-oriented.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Notes
Tested and working on Fedora 37

## Requirements
- [x] Python 3 (Preferably 3.10)
- [x] python3-pip

## Installation and Setup
1. Download this project with `git clone https://github.com/PhysCorp/Pydoctor-Plus.git`
2. Install the requirements with `python3 -m pip install -r requirements.txt`.
3. Move all of the folders and files from `.vscode` and `api` to the root of your project.
4. (If you haven't already) Download and install the [Task Runner Extension](https://marketplace.visualstudio.com/items?itemName=SanaAjani.taskrunnercode) for VSCode.
5. When ready to generate pydoctor documentation for your project, open the `Task Runner` menu on the left-hand side of the screen and click the `Compile API Documentation from Project Folder` task. The documentation will be generated in the `docs` folder in your project directory, separated into each python file path.
6. Next, run the `Link Together ALL API Doc Files` task in Task Runner to link all of the files together into one file. The file will be located in the `docs` folder in your project directory, named `index.html`.
7. Profit!

## Additional Configuration
Please check out the files in `.vscode` and `api` to see what you can change to fit your needs. For example, you can specify the name of the linked HTML document inside of `link_documentation.sh` in the `api/scripts` folder.
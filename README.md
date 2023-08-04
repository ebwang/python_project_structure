# python_project_structure
Guid to Use Python Projects<br>

1- Configure Pyenv to configure the version of python<br>
pyenv install --list | grep " 3\.[678]"<br>
pyenv install -v 3.11.2<br>
Install desired version but now you have to select:<br>
pyenv versions<br>
List all versions installed<br>
pyenv local 3.11.2<br>
Finally create .venv<br>
python3 -m venv .venv<br>

2- Install poetry inside the project to get the new version of python<br>
First need to install: pip install poetry
poetry init<br>
poetry add pkg<br>
poetry add --dev pkg<br> 
OBS: When you use this flag, this package will only aveilable in test isolated from prod.<br>
Remember if you upoad the poetry.lock you can reproduce the exactly enviroment

3- Initalize with git and generate gitignore<br>
https://www.toptal.com/developers/gitignore/<br>

4- Always implement tests<br>
OBS: Remember to dunder init the folder test<br>
Remember Coverage pytestcoverage<br>

5- Lint the code and check security<br>
prospector<br>
flake8(Already included in prospector<br>
autopep8(Included in vscode)<br>
blue<br>

6-Pip-Audit to scan vulnerabilities<br>
pip-audit<br>

7-Documentation MkDocs<br>
poetry add --group docs mkdocs mkdocs-material
poetry add --docs mkdocs-material<br>
poetry add --docs mkdocstrings<br>
poetry add --docs mkdocstrings-python<br>

Run:<br>
mkdocs new . <br>
Will create the strcture and a folder called docs<br>
mkdocs server -> Will start a webpage containing the docs<br>

Put the sample files:
explanation.md  how-to-guides.md  index.md  reference.md  tutorials.md

Build with the mkdocs.yml outside the folder docs
mkdocs build

Ater the build will show the html pages in site folder



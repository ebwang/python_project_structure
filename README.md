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
poetry init<br>
poetry add pkg<br>
poetry add --dev pkg<br>

3- Initalize with git and generate gitignore<br>
https://www.toptal.com/developers/gitignore/<br>

4- Always implement tests<br>
OBS: Remember to dunder init the folder test<br>

5- Lint the code and check security<br>
prospector<br>
flake8(Already included in prospector<br>
autopep8(Included in vscode)<br>

6-Pip-Audit to scan vulnerabilities
pip-audit





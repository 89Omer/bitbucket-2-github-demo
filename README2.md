# Contributions-Importer-For-Github/run_script.py
import git
from git_contributions_importer import *

# Your private repo or Bitbucket repo
repo = git.Repo("path/to/repo")
# Your mock repo
mock_repo = git.Repo("path/to/your/mock-repo")
importer = Importer([repo], mock_repo)
# I use both my personal email and work email here,
# Since the private repo uses work email, and Github uses my personal email
importer.set_author(['personal@email.com', 'work@company.com'])
importer.import_repository()

# Install gitpython and pathlib with pip3

pip3 install gitpython
pip3 install pathlib

# You must run the script with python3

python3 run_script.py


# If you see a bunch of logs running with analysing commits, you got it.
 
# Don’t forget to push changes from your mock repo to Github.
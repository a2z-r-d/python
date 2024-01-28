# python

```
# create virtual env
python3 -m venv project_env
# Activate python virtual evn
source project_env/bin/activate

# to see which python env is working on
which python

# To install a mocule like requires and pytz
pip install requires
pip install pytz

# To list module
pip list

# To create requirements.txt

pip freeze > requirements.txt

# To diactivate current virtual environment
deactivate

# To delete virtual environment simple delete the directory

rm -rf project_env/

# Some good practice
# Create a folder for the project
mkdir my_project
# Create virtual environment into the folder of the project created earlier
python3 -m venv my_project/venv
# Then activate the venv into the project
source my_project/venv/bin/activate
```

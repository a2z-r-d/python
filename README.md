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

# Now install packages/modules from the requirements.txt file
pip install -r requirements.txt


# To get access to the global packages
python3 -m venv venv --system-site-packages

source venv/bin/activate
# Now do pip list it will list all the package installed globally

(venv) my_project$ pip list

# The output is given below

Package            Version
------------------ ----------
certifi            2023.11.17
charset-normalizer 3.3.2
idna               3.6
pip                23.2.1
requests           2.31.0
urllib3            2.1.0

[notice] A new release of pip is available: 23.2.1 -> 23.3.2
[notice] To update, run: pip install --upgrade pip

# By this way if you install additional packages after activating the virtual environment
# It will not install or affect to the global packages.

# To list the packages only installed in activated virtual environment is below:
pip list --local


# Example of installing and listing only packages are installed in local
(venv) my_project$ pip install flux
Collecting flux
  Downloading flux-1.3.5.tar.gz (13 kB)
  Installing build dependencies ... done
  Getting requirements to build wheel ... done
  Installing backend dependencies ... done
  Preparing metadata (pyproject.toml) ... done
Building wheels for collected packages: flux
  Building wheel for flux (pyproject.toml) ... done
  Created wheel for flux: filename=flux-1.3.5-py3-none-any.whl size=6255 sha256=4bf4fba9c2e3cf18922e7e95b4c3cc9752d173d2ca34c0afc3b4affede25ca51
  Stored in directory: /Users/assad/Library/Caches/pip/wheels/42/08/f8/48bb835135176d37a94cd76f50f3839f8e6ac91e783b4ba96c
Successfully built flux
Installing collected packages: flux
Successfully installed flux-1.3.5

[notice] A new release of pip is available: 23.2.1 -> 23.3.2
[notice] To update, run: pip install --upgrade pip
(venv) my_project$ pip list --local
Package Version
------- -------
flux    1.3.5
pip     23.2.1

[notice] A new release of pip is available: 23.2.1 -> 23.3.2
[notice] To update, run: pip install --upgrade pip




```

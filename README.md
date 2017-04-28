## Jupyter Playground

Set up a virutalenv for `python3`

> virtualenv .env -p /bin/python3

Activate this virtualenv

> source .env/bin/activate

Check if python from virtualenv is activate

> which python

should display
> ==> /path/to/repo/.env/bin/python

Install all the dependencies

> pip install -r requirements.txt

Generate password for your jupyter

> python -c 'from notebook.auth import passwd; print(passwd())'

Replace the password hash in `.jupyter/jupyter_notebook_config.py` (@Line 218)

Start Jupyter

> jupyter notebook --config=.jupyter/jupyter_notebook_config.py

Enter your password when prompted

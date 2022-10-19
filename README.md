# How to run this repo locally

*Note

## Prequisites
* Install and run virtualenv to create a virtual environment
```
# install virtualenv
pip install virtualenv

# Create your environment
virtualenv env

# Activate the environment
# On Windows
./env/Scripts/activate

# On Unix-based OS
source .env/bin/activate

# Download the required packages
pip install -r requirement.txt
```

## Run the project
```
# On first run, you will need to
# create an admin account to manage the server (optional) and
# migrate the Database
python manage.py createsuperuser

python manage.py migrate

# Start the application (Development mode)
python manage.py runserver

# The application now can be accessed at 127.0.0.1:8000 in your browser
# You can run the app on a custom port with:
python manage.py runserver 0.0.0.0:<your_port>
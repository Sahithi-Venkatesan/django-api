# task
It's an API in Django using Postman

To run the file locally
Install the prerequisites:

Use the following command

    sudo apt install python3 python3-pip virtualenv libpq-dev python3-dev build-essential postgresql-server-dev-all

Then use the command:

    ./start

If the above command fails:

1)  Use the command
    
        ./venv/bin/activate

2)If venv does not exist => create it

    virtualenv -p python3 venv
    
3)Activate venv and install the requirements

    pip install -r requirements.txt
    
4)Make and migrate the db

    python manage.py makemigrations
  
    python manage.py migrate
  
5)Static files

    python manage.py collectstatic
  
6)Start the server

    python manage.py runserver

# Django RestAPI


## Technologies used
* [Django](https://www.djangoproject.com/): The web framework for perfectionists with deadlines (Django builds better web apps with less code).
* [DRF](www.django-rest-framework.org/): A powerful and flexible toolkit for building Web APIs

# Task Description
Implementing authentication in a DRF API
We'll be creating a bucket list API. If you haven't heard about the term bucket list, it is a list of all the goals you want to achieve, dreams you want to fulfill and life experiences you desire to experience before you die (or hit the bucket). This API should therefore help us to create and manage our bucketlists.

The API will have the ability to do following things:

- Create a Bucketlist
- Retrieve a Bucketlist
- Update it
- Delete one's bucketlist
- Authentication of API Users

## Http Methods:

    - Create a bucketlist – Handle POST request
    - Read a bucketlist(s) – Handle GET request
    - Update a bucketlist – Handle PUT request
    - Delete a bucketlist – Handle DELETE request

## Installation
* If you wish to run your own build, first ensure you have python globally installed in your computer. If not, you can get python [here](https://www.python.org").
* After doing this, confirm that you have installed virtualenv globally as well. If not, run this:
    ```bash
        $ pip install virtualenv
    ```
* Git clone this repo to your PC 
    ```bash
        $ git clone https://github.com/virenkapadia07/django-rest-api.git
    ```

* #### Dependencies

    1. cd into your the cloned repo as such:
        ```bash
            $ cd django-rest-api
        ```
    2. Create and fire up your virtual environment:
        ```bash
            $ virtualenv  venv -p python3
            $ source venv/bin/activate
        ```
    3. Install the dependencies needed to run the app:
        ```bash
            $ pip install -r requirements.txt
        ```
    4. Make those migrations work
        ```bash
            $ python manage.py makemigrations
            $ python manage.py migrate
        ```
    5. Create a User to get authenticated
        ```bash
            $ python manage.py createsuperuser
        ```

    6. Test your project is working proper or not
        ```bash
            $ python manage.py test
            $ python manage.py test api
        ```

* #### Run It
    Fire up the server using this one simple command:
    ```bash
        $ python manage.py runserver
    ```
    You can now access the file api service on your browser by using
    ```
        http://localhost:8000/api/bucketlists/
    ```


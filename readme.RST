0. Pull this and fetch the submodules: :code:`git submodule update --init`

1. Train rasa: :code:`rasa train`

2. Launch rasa action server: :code:`rasa run actions`

3. In a separate process run rasa API: :code:`rasa run --enable-api`

4. Set :code:`.env` file from :code:`.env.example` with your twilio credentials and phone to send stuff (INPHONE) and registered phone to send TO (OUTPHONE)

5. Run :code:'python manage.py createsuperuser' to create an access to admin pages

6. Run :code:`python manage.py runserver`

6.1. Run :code:`./ngrok http 8000`

6.2. In Twilio console add the ngrok address + :code:`/med/` to the SMS redirect

7. Go to :code:`localhost:8000`.

8. Add new request to the :code:`requests` table.

9. Enjoy :)

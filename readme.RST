0. Pull this and fetch the submodules: `git submodule update --init`
1. Train rasa: `rasa train`
2. Launch rasa action server: `rasa run actions`
3. In a separate process run rasa API: `rasa run --enable-api`
4. Set `.env` file from `.env.example` with your twilio credentials and phone to send stuff (INPHONE) and registered phone to send TO (OUTPHONE)
5. Run 'python manage.py createsuperuser' to create an access to admin pages
6. Run `python manage.py runserver`
7. Go to `localhost:8000`.
8. Add new request to the `requests` table.
9. Enjoy :)

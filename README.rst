=====
Polls
=====

Polls is a thing which does things.
Polls does polls.
Polls.

BTW the actual package is in "./dist/"
I only uploaded the whole thing to GitHub so you can see what a Django package
looks like.

Quick start
-----------

0. If not installed, install polls from here with::

   python -m pip install --user ./dist/polls-packaged-0.1.tar.gz

1. Add "polls" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'polls',
    ]

2. Include the polls URLconf in your project urls.py like this::

    path('polls/', include('polls.urls')),

3. Run ``python manage.py migrate`` to create the polls models.

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a poll (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/polls/ to get right in about the poll.

django-report-builder
=====================

A GUI for Django ORM. Build custom queries and display results. 
Targets sys admins and capable end users who might not be able to program or gain direct interactive shell access.

[![Build Status](https://travis-ci.org/burke-software/django-report-builder.png?branch=master)](https://travis-ci.org/burke-software/django-report-builder) [![Bountysource](https://www.bountysource.com/badge/tracker?tracker_id=314767)](https://www.bountysource.com/trackers/314767-burke-software-django-report-builder?utm_source=314767&utm_medium=shield&utm_campaign=TRACKER_BADGE)

[Support development on gratipay](http://www.gratipay.com/bufke)

# News

We now have a [google group](https://groups.google.com/forum/#!forum/django-report-builder/). Please post suggestions, ask questions, and let me know how you're using django report builder. I'll make future announnments there.

# What is Django Report Builder?

![](docs/screenshots/reportbuilderscreen.png)

## Features

- Add filters
- Add display fields
- Preview and create xlsx reports
- Very simple security, user must have change or "view" permission to view 
reports. Unprivileged users can still build reports and see database schema.
- Model properties (thanks yekibud)
- Support for [django-custom-fields](https://github.com/burke-software/django-custom-field)
- Support for django-hstore
- Export to Report global admin action
- Optional asynchronous report generation

# Documentation

http://django-report-builder.readthedocs.org/

# Hacking

We've included a fig.yml file for use with [fig](http://fig.sh/). There's also a demo project so you can start using report builder right now without touching any python code.
Once you have fig installed just run `fig up`. Populate the database with `fig run --rm web ./manage.py migrate`. 
You may want to edit fig.yml to comment/uncomment the django-report-utils line. Report utils is a seperated library with common reporting functions. If you want to hack on report utils too just clone the repo in a sibling directory.

# Discussion

Let us know your thoughts at https://google.com/+Burkesoftware

[2.x]: https://github.com/burke-software/django-report-builder/tree/2.x

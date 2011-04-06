# ANDORIA | MLC's Admissions Application Application #

Don't ask about the name, I know it doesn't make sense.

## Purpose ##

Andoria is the online web application written specifically to handle admission applications for Martin Luther College. It will start as an undergraduate-only piece of software, but the future will hopefully bring more functionality and handle all manner of applications for different departments at the school.

## Technology ##

* Rails 3.0.x
* SQLite 3.x
* PostgreSQL 8.x
* Ruby 1.9.x

Rails provides the background framework for the whole thing while SQLite provides a place to store any applications that are not immediately submitted for approval. Upon approval, they are stored in the CWDB (campus-wide database) which uses PostgreSQL at the moment. Everything runs on top of Ruby 1.9. No important information is stored in the SQLite database which is stored directly on the web server, that information (like social security numbers, birthdate, etc.) are transmitted only at the time of submission and put directly into the CWDB where it can be more securely stored.
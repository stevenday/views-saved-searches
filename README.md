views-saved-searches
====================

Saved (Views) Searches Module for Drupal 6/Views 2

Allows users with the appropriate permissions to save a configuration of exposed
filters in Views 2, and then access them at any time from a tab on their user
page.

The optional sub-module - views saved searches alerts, lets users also sign up
to receive email 'alerts' from their saved searches, where new nodes which
match their criteria are emailed to them. Currently this is fixed to occur daily
on a cron job.

The saved search details are also exposed to views, with some custom ajax 
control fields, so that you can build your own interface.

Installation
------------
Enable the module on the modules page as normal, configuration of which views to
allow searches to be saved and is done via the admin settings pages:
      admin/settings/views-saved-searches
      admin/settings/views-saved-searches/alerts
and you also need to make sure you give the permission to save searches and 
receive alerts to the right roles.

Requires:
* Drupal 6
* Views 2
* cron

Works best when you have the job_queue module installed as well so that it can
queue up tasks and then work with whatever cron schedule you have setup.
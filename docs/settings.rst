.. _settings:

Settings
========

You can configure some of the application behaviour with the ``WGER_SETTINGS``
dictionary in your settings file. Currently, the following options are supported:

**ALLOW_REGISTRATION**: Default ``True``.
  Controls whether users can register on their own or if a gym administrator has
  to create the user accounts.

**ALLOW_GUEST_USERS**: Default ``True``.
  Controls whether users can use the site as a guest user or if an administrator
  has to create the user accounts, as with the option above.

**USE_RECAPTCHA**: Default ``False``.
  Controls whether a captcha challenge will be presented when new users register.

**REMOVE_WHITESPACE**: Default ``False``.
  Removes whitespaces around HTML tags to reduce the size of the resulting HTML.
  If you are not serving the site using TLS you probably want to use the GZip
  middleware instead. Read the Django documentation on the security implications
  (BREACH attack).

**EMAIL_FROM**: Default `wger Workout Manager <wger@example.com>`
  The sender address used for sent emails by the system such as weight reminders


.. note::
  If you want to override a default setting, don't overwrite all the dictionary
  but only the keys you need, e.g. ``WGER_SETTINGS['foo'] = 'bar'``. This avoids
  problems when new keys are added in the global settings.

Set the URL for your site in the table ``django_site``. This is only used e.g. in
the password reset emails.

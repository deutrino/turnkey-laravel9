Laravel - PHP Framework
=======================

`Laravel`_ is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable, creative experience to be truly fulfilling. Laravel attempts to take the pain out of development by easing common tasks used in the majority of web projects, such as authentication, routing, sessions, and caching.

This appliance includes all the standard features in `TurnKey Core`_, and on top of that:

- Laravel 
  
   - Installed from upstream source to /var/www/laravel
   - Composer globally installed for all your projects

- SSL support out of the box.
- `Adminer`_ administration frontend for MySQL (listening on port 12322 - uses SSL).
- Postfix MTA (bound to localhost) to allow sending of email (e. g. password recovery).
- Webmin modules for configuring Apache2, PHP, MySQL and Postfix.


How to use Laravel
-------------------------------------------

To update Laravel:

    cd /var/www/laravel
    
    composer self-update
    
    composer update

Laravel Documentation: http://laravel.com/docs/5.1

Credentials *(passwords set at first boot)*
-------------------------------------------

-  Webmin, SSH, MySQL, Adminer: username **root**


.. _Laravel: http://laravel.com
.. _TurnKey Core: https://www.turnkeylinux.org/core
.. _Adminer: http://www.adminer.org

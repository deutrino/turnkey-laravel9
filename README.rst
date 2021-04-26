Laravel - PHP Framework for Web Artisans
========================================

`Laravel`_ is a web application framework with expressive, elegant syntax. We
believe development must be an enjoyable, creative experience to be truly
fulfilling. Laravel attempts to take the pain out of development by easing
common tasks used in the majority of web projects, such as authentication,
routing, sessions, and caching.

This appliance includes all the standard features in `TurnKey Core`_, and on top of that:

- Laravel 
  
   - Latest LTS_ release installed via composer_ to /var/www/laravel.
   - Composer_ globally installed for all your projects.
   - Includes turnkey-composer_ and turnkey-artisan_ (wrapper scripts which
     run composer_ and artisan_ respectively; as www-data user).

- SSL support out of the box.
- `Adminer`_ administration frontend for MySQL (listening on port 12322 - uses SSL).
- Postfix MTA (bound to localhost) to allow sending of email (e. g. password recovery).
- Webmin modules for configuring Apache2, PHP, MySQL and Postfix.

Usage
-----

`Laravel Documentation`_

Update Laravel::

    cd /var/www/laravel
    # update composer
    composer self-update
    # update laravel build
    turnkey-composer update

If you wish to update to a newer release of Laravel (i.e. not the currently
installed LTS) then please consult the `Laravel Upgrade Documentation`_.

Credentials *(passwords set at first boot)*
-------------------------------------------

-  Webmin, SSH, MySQL: username **root**
-  Adminer: username **adminer**


.. _Laravel: https://laravel.com
.. _TurnKey Core: https://www.turnkeylinux.org/core
.. _LTS: https://laravel.com/docs/releases#support-policy
.. _composer: https://getcomposer.org/
.. _turnkey-composer: https://github.com/turnkeylinux/common/blob/master/overlays/composer/usr/local/bin/turnkey-composer
.. _artisan: https://laravel.com/docs/artisan
.. _turnkey-artisan: https://github.com/turnkeylinux/common/blob/master/overlays/artisan/usr/local/bin/turnkey-artisan
.. _Adminer: https://www.adminer.org
.. _Laravel Documentation: https://laravel.com/docs/6.x
.. _Laravel Upgrade Documentation: https://laravel.com/docs/upgrade

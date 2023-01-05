Pixelfed - decentralized social photo sharing
=============================================

`Pixelfed`_ is a fresh take on photo sharing. Get inspired with beautiful
photos captured by people around the world. Connect instantly with
millions of users on the global ActivityPub Fediverse.

- Ad-free and privacy friendly
- Open source and decentralized
- Chronological feeds 

This appliance includes all the standard features in `TurnKey Laravel`_, and on top of that:

- latest Pixelfed
- Laravel 9.x
   - Latest 9.x_ release installed via composer_ to /var/www/laravel.
- PHP 8.1
   - Composer_ globally installed for all your projects.
   - Includes turnkey-composer_ and turnkey-artisan_ (wrapper scripts which
     run composer_ and artisan_ respectively; as www-data user).

- SSL support out of the box.
- `Adminer`_ administration frontend for MySQL (listening on port 12322 - uses SSL).
- Postfix MTA (bound to localhost) to allow sending of email (e. g. password recovery).
- Webmin modules for configuring Apache2, PHP, MySQL and Postfix.

Usage
-----

`Pixelfed Documentation`_

TODO


`Laravel Documentation`_

Update Laravel::

    cd /var/www/laravel
    # update composer
    composer self-update
    # update laravel build
    turnkey-composer update

If you wish to update to a newer release of Laravel then please consult the
`Laravel Upgrade Documentation`_.

Credentials *(passwords set at first boot)*
-------------------------------------------

-  Webmin, SSH, MySQL: username **root**
-  Adminer: username **adminer**


.. _Pixelfed: https://pixelfed.org
.. _Unofficial TurnKey Laravel 9: https://github.com/deutrino/turnkey-laravel9
.. _composer: https://getcomposer.org/
.. _turnkey-composer: https://github.com/turnkeylinux/common/blob/master/overlays/composer/usr/local/bin/turnkey-composer
.. _artisan: https://laravel.com/docs/artisan
.. _turnkey-artisan: https://github.com/turnkeylinux/common/blob/master/overlays/artisan/usr/local/bin/turnkey-artisan
.. _Adminer: https://www.adminer.org
.. _Laravel Upgrade Documentation: https://laravel.com/docs/upgrade

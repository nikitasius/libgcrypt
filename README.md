# libgcrypt
libgcrypt library for [GnuPG](https://github.com/nikitasius/GnuPG/) with 32kb RSA keys.

# Description
This library based on original [libgcrypt 1.6.5](https://gnupg.org/ftp/gcrypt/libgcrypt/libgcrypt-1.6.5.tar.bz2). Original version of libgcrypt 1.6.5 was copied into the branch [libgcrypt-1.6.5](https://github.com/nikitasius/libgcrypt/tree/libgcrypt-1.6.5) and after was copied into branch devel, where was modified. And complete version was moved into branch [libgcrypt-1.6.5-RSA32k](https://github.com/nikitasius/libgcrypt/tree/libgcrypt-1.6.5-RSA32k).

# Configuration
Run `./configure` or `./configure --help` in case if you want custom configuration.

# Compilation
Run `make`, if no errors, run `make check`.

# Installation
If all tests passed, run `checkinstall`

>1 -  Summary: [ libgcrypt-1.6.5 ]

>2 -  Name:    [ libgcrypt ]

>3 -  Version: [ 1.6.5 ]

>11 - Provides: [ libgcrypt ]

or run `make install` in case if you do not use `checkinstall`.

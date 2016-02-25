# libgcrypt
###libgcrypt library for [GnuPG](https://github.com/nikitasius/GnuPG/) with 32kb RSA keys.
## WARNING
## USE MODIFIED LIBGCRYPT AT YOUR OWN RISK. SOFTWARE MAY CAUSE DATA LOSS, SYSTEM CRASHES, AND RED EYES.
### Large keys, created in modified GnuPG with modified libgcrypt CANNOT be read by vanilla versions! It mean, that if you have another PGP stuff in your PC which work with keys, you should to export keys OR create another keyring for vanilla versions.

## Description
This library based on original [libgcrypt 1.6.5](https://gnupg.org/ftp/gcrypt/libgcrypt/libgcrypt-1.6.5.tar.bz2). Original version of libgcrypt 1.6.5 was copied into the branch [libgcrypt-1.6.5](https://github.com/nikitasius/libgcrypt/tree/libgcrypt-1.6.5) and after was copied into branch **devel**, where was modified. And complete version was moved into branch [1.6.5-RSA32k](https://github.com/nikitasius/libgcrypt/tree/1.6.5-RSA32k).

## Configuration
### Patching vanilla gnupg-2.0.29
If by some private reasons you don't want to download this version from this Github repo, you can download patch [libgcrypt-1.6.5-RSA32k.patch](https://raw.githubusercontent.com/nikitasius/libgcrypt/1.6.5-RSA32k/libgcrypt-1.6.5-RSA32k.patch) and download [vanilla libgcrypt-1.6.5](https://gnupg.org/ftp/gcrypt/libgcrypt/libgcrypt-1.6.5.tar.bz2).

After you can check patch content and if all is ok, copy it inside folder with vanilla libgcrypt-1.6.5 and run `patch -p1 < libgcrypt-1.6.5-RSA32k.patch`. After patching your libgcrypt-1.6.5 will be able to work with RSA-32768 keys.

### Debian
Run `./configure` or `./configure --help` in case if you want custom configuration.

## Compilation
Run `make`, if no errors, run `make check`.

## Installation
If all tests passed, run `checkinstall`

>1 -  Summary: [ libgcrypt-1.6.5 ]

>2 -  Name:    [ libgcrypt ]

>3 -  Version: [ 1.6.5 ]

>11 - Provides: [ libgcrypt ]

or run `make install` in case if you do not use `checkinstall`.

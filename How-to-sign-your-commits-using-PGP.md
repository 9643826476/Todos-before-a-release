# Git signing on Windows

## Prerequisites

1. Install [gpg4win](https://www.gpg4win.org/)
1. Install [Git](https://git-scm.com/download/win)

*Note: Make sure to install the Git bash component* 

## PGP

Open a Git Bash shell window and check if your key is available:

```bash
$ gpg --list-keys
```

If it isn't, then import your combined private + public key with this command:

```bash
$ gpg --import /path/to/yourkey.pub-sec.asc
gpg: key NCB0X317: public key "Nextcloud Packager <nextcloudpackager@nextcloud.com>" imported
gpg: key NCB0X317: secret key imported
gpg: key NCB0X317: "Nextcloud Packager <nextcloudpackager@nextcloud.com>" 1 new signature
gpg: Total number processed: 2
gpg:               imported: 1  (RSA: 1)
gpg:         new signatures: 1
gpg:       secret keys read: 1
gpg:   secret keys imported: 1
```

Trust the key by typing the following:

```bash
$  gpg --edit-key "Nextcloud Packager" trust quit
```

Answer `5`: I trust ultimately and confirm with `y`.

*Note: You can do all of this from the Kleopatra app if you prefer*

## Git

Add your full name and email address

```bash
$ git config --global user.name Nextcloud Packager (ncpkger)
$ git config --global user.email nextcloudpackager@nextcloud.com
```

Let git use the pinentry app which comes with gpg4win

```bash
$ git config --global gpg.program "c:/Program Files (x86)/GNU/GnuPG/gpg2.exe"
```

Tell git to always sign your commits:

```bash
git config --global commit.gpgsign true
```

Add your key to git by first listing your key and memorizing the alphanumerical sequence after 4096R/:

```bash
$ gpg --list-keys
/c/Users/nextcloud/.gnupg/pubring.gpg
----------------------------------
pub   4096R/NCB0X317 2016-01-01 [expires: 2020-01-01]
uid                  Nextcloud Packager <nextcloudpackager@nextcloud.com>
sub   4096R/BOXFTW16 2016-08-13 [expires: 2021-08-12]
```

and then linking that key to your git user

```bash
git config --global user.signingkey NCB0X317 
```

That's it! You should now be able to sign your commits using your GPG key.

## Testing

Create a test commit from your IDE or the command line.
You should see a window poping up, asking for your password.

Back in Git Bash, you can check your signature by typing:

```bash
$  git log 45cf201 --show-signature -1
commit 45cf201ac70f8acc06916184c4e2392cdfa05467
gpg: Signature made 09/28/16 23:33:56 W. Europe Summer Time
gpg:                using RSA key 123E4567NCB0X317
gpg: Good signature from "Nextcloud Packager <nextcloudpackager@nextcloud.com>" [ultimate]
Author: Nextcloud Packager (ncpkger) <nextcloudpackager@nextcloud.com>
Date:   Wed Sep 28 23:33:38 2016 +0200

    Create a test signature for our contributors
```

# Git signing on Linux

TBW

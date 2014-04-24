backupscript
============

Postgresql Backup Script

This script is intended to be used as a cron job.

Why it uses a temp directory?

Because it is also intended to be used along with Dropbox sync feature or any similar software. If we don't use a temp directory then Dropbox will start to sync files before being encrypted.

Do I need GnuPG?

If you want your files to be encrypted then yes, you do. If you leave the RECIPIENT variable empty then no files will be encrypted.

Can I backup more than one database?

Yes, you can. You must set them as a whitespace separated list. All databases must be owned by the same user and password.

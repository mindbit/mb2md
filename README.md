# Convert Mbox mailboxes to Maildir format

**The initial version of this script was downloaded from:
http://dovecot.org/tools/mb2md.pl**

This version was modified for Dovecot. Additional changes and bugfixes
have been made by Mindbit SRL.

Original author and copyright information (can also be found in the
script file):

> Public domain.
>
> currently maintained by:
> Juri Haberland <juri@koschikode.com>
> initially wrote by:
> Robin Whittle
>
> This script's web abode is http://batleth.sapienti-sat.org/projects/mb2md/ .
> For a changelog see http://batleth.sapienti-sat.org/projects/mb2md/changelog.txt
>
> The Mbox -> Maildir inner loop is based on  qmail's script mbox2maildir, which
> was kludged by Ivan Kohler in 1997 from convertandcreate (public domain)
> by Russel Nelson.  Both these convert a single mailspool file.
>
> The qmail distribution has a maildir2mbox.c program.

## What is does:

Reads a directory full of Mbox format mailboxes and creates a set of
Maildir format mailboxes.  Some details of this are to suit Courier
IMAP's naming conventions for Maildir mailboxes.

http://www.inter7.com/courierimap/

This is intended to automate the conversion of the old
/var/spool/mail/blah file - with one call of this script - and to
convert one or more mailboxes in a specifed directory with separate
calls with other command line arguments.

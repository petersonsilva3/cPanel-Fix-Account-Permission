# cPanel Fix Account Permission

This is a simple bash script I wrote to fix the permissions and ownership of files within a cpanel account.
To use, simply copy the script your server, chmod 755, and pass the usernames as arguments:

    ./fixperms user1 user2 user3

You can also run a server-wide loop like this:

    for i in `ls -A /var/cpanel/users` ; do ./fixperms $i ; done

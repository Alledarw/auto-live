# auto-live
A test repo for CD exercise with GitHub Actions on an nginx server.
Automatically pull to the repo on the web server (var/www/ ) when a new push is made.

Example repository:

https://github.com/alledarw/auto-live

Don't forget to add the correct secrets in GitHub by going to:
Settings > Secrets and variables > Actions > Repository Secrets and adding them (with the same names as in your GitHub Actions workflow).

Afterwards:

Change your nginx settings in /etc/nginx/sites-enabled/reverseproxy so that you serve the directory /var/www/auto-live under one of your domains.

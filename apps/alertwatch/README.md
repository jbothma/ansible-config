# Initial setup

1. run the playbook
2. set up the DNS record
3. create the postgres DB (using dokku-postgres on a hetzner volume for now)
4. link the postgres db to the app
5. Enable dokku letsencrypt for the app
6. Enable the dokku letsencrypt cron job for the app
7. push the app to the dokku git remote
8. Run migrations
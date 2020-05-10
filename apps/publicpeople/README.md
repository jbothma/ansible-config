Configure the app on the server using Ansible

    ansible-playbook --start-at-task "Dokku app exists" playbook.yml

Set up the database on the server

    dokku postgres:create publicpeople
    cat some-db-dump.custom | dokku postgres:import publicpeople
    dokku postgres:link publicpeople publicpeople

Push the code to the server from a git clone. You can get the git remote from\\
the output of the playbook above. Assuming you added the remote as `dokku`

    git push dokku master
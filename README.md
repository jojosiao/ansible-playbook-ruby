# Ansible Playbook Ruby

It installs:

- Ruby 2.3.1
- PostgreSQL 9.5.4
- Nginx
- Puma (jungle)

1. Change the app name and deploy directory in <code>vars/defaults.yml</code>.
2. Rename `hosts.example` to `hosts` and change it to your hosts.

To run:

    $ ansible-playbook -i hosts ruby-webapp.yml -t ruby,deploy,postgresql,nginx
    $ <deploy your app>
    $ ansible-playbook -i hosts ruby-webapp.yml -t puma

There is an example Capistrano `deploy.rb` in this repository that you can use too.


## Credits



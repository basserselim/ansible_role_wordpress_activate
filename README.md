Role Name
=========

This roles uses the wordpress-cli to activate a list of plugins and a specified theme

Requirements
------------

- wordpress
- wordpress-cli

Role Variables
--------------
* `wordpress_activate_plugins`: a list of plugins to activate
* `wordpress_activate_theme`: the name of the theme to activate
* `wordpress_activate_path`: the directory where wordpress is installed

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: basserselim.wordpress_activate
           wordpress_activate_plugins:
             - 'wp-updates-notifier'
             - 'rest-api'
           wordpress_activate_theme: 'twenty-eleven' 
           wordpress_activate_path: "/var/www/wordpress"

License
-------

BSD

Author Information
------------------

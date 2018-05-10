# symfony3.4-crud-with-easyadmin-and-relations
symfony3.4 crud with easyadmin and relations with user and customer

Basic requirements: PHP 7.0, MySQL, Apache, rewrite moduel enabled. composer, git 

clone the project and update the file (app\config\parameters.yml) with db credentials and then run the command:

php bin/console doctrine:schema:update --force

After that we would need one User with ROLE_ADMIN credentials to access our admin application. This can be done with two simple Symfony2 shell and FOSUser commands:
 
php bin/console fos:user:create admine admin@me.com admine
php bin/console fos:user:promote admine ROLE_ADMIN
 

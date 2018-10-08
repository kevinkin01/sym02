# sym02
##Website-skeleton

### work process

### update dependencies
1) composer update
### server
php bin/console server:run

###modify .env
1)change . env with DB connection :DATABASE_URL=mysql://root:@127.0.0.1:3306/sym_02 

2) the future DB will be sym_02

### install security-checker for composer
1) composer require sensiolabs/security-checker --dev
2) test it with : composer update

### create DB
php bin/console doctrine:database:create

### create an antity like a table for mysql
php bin/console make:entity
>article
>titre
>? view al suggestion
>string
>150
>no
>description
>text
>no
>temps
>datetime
>yes
>auteur
>string
>no

### prepare SQL in  a migration file in MYSQL
php bin/console make:migration
### real migrations
php bin/console doctrine:migrations:migrate

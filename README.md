# Start

```
wunder@code2018-VirtualBox:~/projects$ composer create-project symfony/skeleton sansay
Installing symfony/skeleton (v4.1.7.3)
  - Installing symfony/skeleton (v4.1.7.3): Downloading (100%)         
Created project in sansay
Loading composer repositories with package information
Installing dependencies (including require-dev) from lock file
Package operations: 20 installs, 0 updates, 0 removals
  - Installing symfony/flex (v1.1.7): Loading from cache
  - Installing psr/cache (1.0.1): Loading from cache
  - Installing psr/container (1.0.0): Loading from cache
  - Installing psr/simple-cache (1.0.1): Loading from cache
  - Installing symfony/polyfill-mbstring (v1.10.0): Loading from cache
  - Installing symfony/console (v4.1.7): Loading from cache
  - Installing symfony/routing (v4.1.7): Loading from cache
  - Installing symfony/http-foundation (v4.1.7): Loading from cache
  - Installing symfony/event-dispatcher (v4.1.7): Loading from cache
  - Installing psr/log (1.0.2): Loading from cache
  - Installing symfony/debug (v4.1.7): Loading from cache
  - Installing symfony/http-kernel (v4.1.7): Loading from cache
  - Installing symfony/finder (v4.1.7): Loading from cache
  - Installing symfony/filesystem (v4.1.7): Loading from cache
  - Installing symfony/dependency-injection (v4.1.7): Loading from cache
  - Installing symfony/config (v4.1.7): Loading from cache
  - Installing symfony/cache (v4.1.7): Loading from cache
  - Installing symfony/framework-bundle (v4.1.7): Loading from cache
  - Installing symfony/yaml (v4.1.7): Loading from cache
  - Installing symfony/dotenv (v4.1.7): Loading from cache
Generating autoload files
Symfony operations: 4 recipes (cbd0df6bb8827b5d899386e80525f5cd)
  - Configuring symfony/flex (>=1.0): From github.com/symfony/recipes:master
  - Configuring symfony/framework-bundle (>=3.3): From github.com/symfony/recipes:master
  - Configuring symfony/console (>=3.3): From github.com/symfony/recipes:master
  - Configuring symfony/routing (>=4.0): From github.com/symfony/recipes:master
Executing script cache:clear [OK]
Executing script assets:install public [OK]

Some files may have been created or updated to configure your new packages.
Please review, edit and commit them: these files are yours.

              
 What's next? 
              

  * Run your application:
    1. Change to the project directory
    2. Create your code repository with the git init command
    3. Run composer require server --dev to install the development web server,
       or configure another supported web server https://symfony.com/doc/current/setup/web_server_configuration.html

  * Read the documentation at https://symfony.com/doc

wunder@code2018-VirtualBox:~/projects$ 
```

after that:

```
wunder@code2018-VirtualBox:~/projects/sansay$ composer require orm-pack
Using version ^1.0 for symfony/orm-pack
./composer.json has been updated
Loading composer repositories with package information
Updating dependencies (including require-dev)
Restricting packages listed in "symfony/symfony" to "4.1.*"

Prefetching 22 packages 🎶 💨
  - Downloading (100%)

Package operations: 23 installs, 0 updates, 0 removals
  - Installing ocramius/package-versions (1.3.0): Loading from cache
  - Installing zendframework/zend-eventmanager (3.2.1): Loading from cache
  - Installing zendframework/zend-code (3.3.1): Loading from cache
  - Installing ocramius/proxy-manager (2.2.2): Loading from cache
  - Installing doctrine/event-manager (v1.0.0): Loading from cache
  - Installing doctrine/cache (v1.8.0): Loading from cache
  - Installing doctrine/dbal (v2.8.0): Loading from cache
  - Installing doctrine/lexer (v1.0.1): Loading from cache
  - Installing doctrine/annotations (v1.6.0): Loading from cache
  - Installing doctrine/reflection (v1.0.0): Loading from cache
  - Installing doctrine/collections (v1.5.0): Loading from cache
  - Installing doctrine/persistence (v1.0.1): Loading from cache
  - Installing doctrine/inflector (v1.3.0): Loading from cache
  - Installing doctrine/common (v2.9.0): Loading from cache
  - Installing doctrine/migrations (v1.8.1): Loading from cache
  - Installing symfony/doctrine-bridge (v4.1.7): Loading from cache
  - Installing doctrine/doctrine-cache-bundle (1.3.5): Loading from cache
  - Installing jdorn/sql-formatter (v1.2.17): Loading from cache
  - Installing doctrine/doctrine-bundle (1.9.1): Loading from cache
  - Installing doctrine/doctrine-migrations-bundle (v1.3.1): Loading from cache
  - Installing doctrine/instantiator (1.1.0): Loading from cache
  - Installing doctrine/orm (v2.6.2): Loading from cache
  - Installing symfony/orm-pack (v1.0.5): Loading from cache
Writing lock file
Generating autoload files
Symfony operations: 4 recipes (dd2b0f2da685562d9122ac3ea4968388)
  - Configuring doctrine/annotations (>=1.0): From github.com/symfony/recipes:master
  - Configuring doctrine/doctrine-cache-bundle (>=1.3.5): From auto-generated recipe
  - Configuring doctrine/doctrine-bundle (>=1.6): From github.com/symfony/recipes:master
  - Configuring doctrine/doctrine-migrations-bundle (>=1.2): From github.com/symfony/recipes:master
ocramius/package-versions:  Generating version class...
ocramius/package-versions: ...done generating version class
Executing script cache:clear [OK]
Executing script assets:install public [OK]

Some files may have been created or updated to configure your new packages.
Please review, edit and commit them: these files are yours.

                        
 Database Configuration 
                        

  * Modify your DATABASE_URL config in .env

  * Configure the driver (mysql) and
    server_version (5.7) in config/packages/doctrine.yaml

wunder@code2018-VirtualBox:~/projects/sansay$ 
```

And after that

```
wunder@code2018-VirtualBox:~/projects/sansay$ ./bin/console doctrine:database
2018-11-13T23:25:11+02:00 [error] Error thrown while running command "'doctrine:database'". Message: "Command "doctrine:database" is not defined.

Did you mean one of these?
    doctrine:cache:clear
    doctrine:cache:clear-collection-region
    doctrine:cache:clear-entity-region
    doctrine:cache:clear-metadata
    doctrine:cache:clear-query
    doctrine:cache:clear-query-region
    doctrine:cache:clear-result
    doctrine:cache:contains
    doctrine:cache:delete
    doctrine:cache:flush
    doctrine:cache:stats
    doctrine:database:create
    doctrine:database:drop
    doctrine:database:import
    doctrine:ensure-production-settings
    doctrine:generate:entities
    doctrine:mapping:convert
    doctrine:mapping:import
    doctrine:mapping:info
    doctrine:migrations:diff
    doctrine:migrations:execute
    doctrine:migrations:generate
    doctrine:migrations:latest
    doctrine:migrations:migrate
    doctrine:migrations:status
    doctrine:migrations:version
    doctrine:query:dql
    doctrine:query:sql
    doctrine:schema:create
    doctrine:schema:drop
    doctrine:schema:update
    doctrine:schema:validate"

                                               
  Command "doctrine:database" is not defined.  
                                               
  Did you mean one of these?                   
      doctrine:cache:clear                     
      doctrine:cache:clear-collection-region   
      doctrine:cache:clear-entity-region       
      doctrine:cache:clear-metadata            
      doctrine:cache:clear-query               
      doctrine:cache:clear-query-region        
      doctrine:cache:clear-result              
      doctrine:cache:contains                  
      doctrine:cache:delete                    
      doctrine:cache:flush                     
      doctrine:cache:stats                     
      doctrine:database:create                 
      doctrine:database:drop                   
      doctrine:database:import                 
      doctrine:ensure-production-settings      
      doctrine:generate:entities               
      doctrine:mapping:convert                 
      doctrine:mapping:import                  
      doctrine:mapping:info                    
      doctrine:migrations:diff                 
      doctrine:migrations:execute              
      doctrine:migrations:generate             
      doctrine:migrations:latest               
      doctrine:migrations:migrate              
      doctrine:migrations:status               
      doctrine:migrations:version              
      doctrine:query:dql                       
      doctrine:query:sql                       
      doctrine:schema:create                   
      doctrine:schema:drop                     
      doctrine:schema:update                   
      doctrine:schema:validate                 
                                               

wunder@code2018-VirtualBox:~/projects/sansay$ 
```

So `doctrine:database:create` command is there as you can see...

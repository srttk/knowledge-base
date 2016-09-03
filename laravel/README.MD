# Laravel

#### Install via Composer

```bash
composer create-project --prefer-dist laravel/laravel blog
```

#### Artisan Commands

##### List all commands

```bash
php artisan list
```

##### List all registered routes
```bash
php artisan routes
```

##### Serve the application on the PHP development server
```bash
php artisan serve
```
##### Change the default port
```bash
php artisan serve --port 8080
```

##### Interact with your application
```bash
php artisan tinker
```
##### Flush the application cache
```bash
php artisan cache:clear
```
##### Database migrations
```bash
php artisan migrate [--bench="vendor/package"] [--database[="..."]] [--path[="..."]] [--package[="..."]] [--pretend] [--seed]
```

### Create a new migration file
```bash
php artisan migrate:make name
```


## DB Seed

### Create Seed
```bash
php artisan make:seed UserTableSeed
```

### Running All Seed
```bash
php artisan db:seed
```

### Running A Specific Seeder class

```bash
php artisan db:seed --class=UserTableSeed
```

## Model
### New Model
```bash
php artisan make:model <modelname>
```
### Generate Model with  Migration
```bash
php artisan make:model <modelname> -m
```

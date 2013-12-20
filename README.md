## Laravel Doctrine

Forked from : https://github.com/atrauzzi/laravel-doctrine/

laravel-doctrine is made by [Alexander Trauzzi](http://goo.gl/QabWv)

#### Installation

Installation is the usual for Laravel packages.

Insert the following in the packages section of your `composer.json` file and run an update:

    "nls/laravel-doctrine": "dev-master",
    
Change your `minimum-stability` to `dev` due to `doctrine-migrations` restrictions :

	"minimum-stability": "dev"

Add the service provider to your Laravel application in `app/config/app.php`. In the `providers` array add:

    'Nls\LaravelDoctrine\LaravelDoctrineServiceProvider',

Then add the following to your `facades` array in the same file:

    'Doctrine' => 'Nls\LaravelDoctrine\Support\Facades\Doctrine',

Publish and edit the default configuration :

    php artisan config:publish nls/laravel-doctrine

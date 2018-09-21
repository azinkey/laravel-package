# laravel-package
Make a fresh start

# Laravel Setup with AdminPanel in 30 minutes
1) composer create-project laravel/laravel <folder>
  
2) SET permission storage/ 

3) SET .env configurations

4) php artisan make:auth

5) php artisan migrate

6) composer require encore/laravel-admin

7) php artisan vendor:publish --provider="Encore\Admin\AdminServiceProvider"

8) php artisan admin:install

9) SET config/admin.php configurations

10) composer require laravel-admin-ext/media-manager -vvv

11) php artisan admin:import media-manager

12) Extension config  config/admin.php         'media-manager' => ['disk' => 'public'],

13) composer require laravel-admin-ext/backup -vvv

14) php artisan admin:import backup

15) composer require laravel-admin-ext/log-viewer -vvv

16) php artisan admin:import log-viewer

17) composer require laravel-admin-ext/config

18) php artisan migrate

19) Open app/Providers/AppServiceProvider.php and call the Config::load() ( use Encore\Admin\Config\Config; )

20) php artisan admin:import config

21) composer require laravel-admin-ext/summernote

22) php artisan vendor:publish --tag=laravel-admin-summernote

23) Extension config in config/admin.php  'summernote' => ['enable' => true, 'config' => ['height' => 500]],

24) php artisan admin:make UserController --model=App\\User

25) Add a route in app/Admin/routes.php： $router->resource('users', UserController::class);

26) php artisan storage:link

27) Add Disk in config/filesystems.php, 'admin' => ['driver' => 'local','root' => storage_path('app/public'),'url' => env('APP_URL').'/storage','visibility' => 'public',], 

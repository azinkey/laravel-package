# laravel-package
Make a fresh start

# Laravel Setup with AdminPanel in 30 minuts
1) composer create-project laravel/laravel <folder>
  
2) SET permission storage/ 

3) SET .env configurations

4) php artisan make:auth

5) composer require encore/laravel-admin

6) php artisan vendor:publish --provider="Encore\Admin\AdminServiceProvider"

7) php artisan admin:install

8) SET config/admin.php configurations

9) composer require laravel-admin-ext/media-manager -vvv

10) php artisan admin:import media-manager

11) Extension config  config/admin.php         'media-manager' => ['disk' => 'public'],

12) composer require laravel-admin-ext/backup -vvv

13) php artisan admin:import backup

14) composer require laravel-admin-ext/log-viewer -vvv

15) php artisan admin:import log-viewer

16) composer require laravel-admin-ext/config

17) php artisan migrate

18) Open app/Providers/AppServiceProvider.php and call the Config::load()

19) php artisan admin:import config

20) composer require laravel-admin-ext/summernote

21) php artisan vendor:publish --tag=laravel-admin-summernote

22) Extension config in config/admin.php  'summernote' => ['enable' => true, 'config' => ['height' => 500]],

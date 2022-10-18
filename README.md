composer require maatwebsite/excel

php artisan migrate:fresh --seed

php artisan make:component users-table

php artisan make:controller ExcelController

php artisan vendor:publish --provider="Maatwebsite\Excel\ExcelServiceProvider" --tag=config

php artisan make:export UsersExport --model=User

php artisan make:import UsersImport --model=User

php artisan migrate:fresh

php artisan optimize:clear

#if you take import errors use below
use GuzzleHttp\Psr7\Request;
and use following Request class instead.
use Illuminate\Http\Request;
I hope it will help you too.


php artisan serve
php artisan make:migration create_tasks_table  database olushturma
php artisan migrate  -databasede table olushturya
php artisan make:model Task --- birinji harpy uly yazylmaly we singular bolmaly
php artisan make:controller TasksController - 
php artisan migrate:fresh --seed
composer install
cp .env.example .env
php artisan key:generate
php artisan config:clear
php artisan migrate
php artisan cache:clear
php artisan passport:install
php artisan passport:install --force
php artisan serve

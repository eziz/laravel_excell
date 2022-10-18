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

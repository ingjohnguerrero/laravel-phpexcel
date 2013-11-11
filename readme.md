## PHPExcel Wrapper for Laravel 4

### Installation

Require package via composer.json

	"rozklad/laravel-phpexcel": "dev-master"

Run composer update
	
	$ composer update

Open __app/config/app.php___ and add ServiceProvider to 'providers' array

		'Rozklad\PHPExcel\ServiceProvider',

Optionally add to aliases

	'Excel'           => 'Rozklad\PHPExcel\Facade',

### Usage

	Excel::fromArray( array(
		array('1', '2', '3'),
		array('X', 'Y', 'Z')
	) )->save( base_path() . '/sample.xls' );

### License

[MIT license](http://opensource.org/licenses/MIT)

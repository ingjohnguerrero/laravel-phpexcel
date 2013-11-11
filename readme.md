## PHPExcel Wrapper for Laravel 4

### Installation

1) Require package via composer.json

	"rozklad/laravel-phpexcel": "dev-master"

2) Run composer update
	
	$ composer update

3) Open __app/config/app.php__ and add ServiceProvider to 'providers' array

	'Rozklad\PHPExcel\ServiceProvider',

4) Optionally add to aliases

	'Excel'           => 'Rozklad\PHPExcel\Facade',

### Usage

	Excel::fromArray( array(
		array('1', '2', '3'),
		array('X', 'Y', 'Z')
	) )->save( base_path() . '/sample.xls' );

### License

[MIT license](http://opensource.org/licenses/MIT)

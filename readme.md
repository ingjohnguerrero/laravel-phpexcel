## PHPExcel Wrapper for Laravel 4

	

### Installation
	
	'Rozklad\PHPExcel\ServiceProvider',

	'Excel'           => 'Rozklad\PHPExcel\Facade',

### Usage

	Excel::fromArray( array(
		array('1', '2', '3'),
		array('X', 'Y', 'Z')
	) )->save( base_path() . '/sample.xls' );

### License

[MIT license](http://opensource.org/licenses/MIT)

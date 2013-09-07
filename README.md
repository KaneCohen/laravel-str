# String manipulation for Laravel 4

Same functionality as core String class, but with correctly and reliably working transliteration.

## Installation

Add following require to your `composer.json` file:

~~~
    "cohensive/str": "dev-master"
~~~

Then run `composer install` or `composer update` to download it and autoload.

In `providers` array you need to add new package:

~~~
'providers' => array(

	//...
	'Cohensive\Str\StrServiceProvider',
	//...

)
~~~

In aliases:

~~~
'aliases' => array(

	//...
	'Str' => 'Cohensive\Str\Facades\Str'
	//...

)
~~~

and comment out:

~~~
	//...
	//'Str' => 'Illuminate\Support\Str'
	//...
~~~

# laravel-ee
elasticemail

.env:
````
ELASTIC_ACCOUNT=
ELASTIC_KEY=
````

````
MAIL_DRIVER=elastic_email
````

 config/services.php:
 ````
 'elastic_email' => [
 	'key' => env('ELASTIC_KEY'),
 	'account' => env('ELASTIC_ACCOUNT')
 ]
 ````
 
 config/app.php:
 ````
  //Illuminate\Mail\MailServiceProvider::class,
  LaravelEE\LaravelElasticEmail\LaravelElasticEmailServiceProvider::class,

 ````

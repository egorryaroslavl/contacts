# Contacts

Installation
------------

```
composer require egorryaroslavl/contacts 
```

Then add ServiceProviders

``` 
  'providers' => [
    // ...
    Egorryaroslavl\Contcts\ContctsServiceProvider::class,
    Collective\Html\HtmlServiceProvider::class,
    Intervention\Image\ImageServiceProvider::class,
    // ...
  ],
```
and aliases 

``` 
  'aliases' => [
    // ...
      'Form' => Collective\Html\FormFacade::class,
      'Html' => Collective\Html\HtmlFacade::class,
      'Image' => Intervention\Image\Facades\Image::class,
    // ...
  ],
``` 
and run
``` 
php artisan vendor:publish 
```


And after all, run this...

```
php artisan migrate
```

  
 

# fixed apis laravel
Como evitar el error Too Many Attemps cuando laravel bloquea los apis

en `app/Http/Kernel.php` laravel tiene por defecto un limite de intentos para todas las rutas apis.
```php

protected $middlewareGroups = [
    ...
    'api' => [
        'throttle:60,1',
    ],
];

```
#### Comentar o inclementar este valor 60 (intentos) , 1 (minutos)

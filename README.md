# Boilerplate para proyectos Laravel

## Requerimientos

- php 8.0

## Features

- Pest (phpunit)
- php-cs-fixer
- phpstan
- roave/security-advisories
- GitHub actions: tests en php 8.0, 8.1. 

## Instalación

```shell
git clone https://github.com/josecl/php-library-boilerplate.git
cd php-library-boilerplate
git remote rm origin
```

Cambiar las referencias, por ejemplo para un proyecto `user/example-project`:

```shell
git remote add origin https://github.com/user/example-project.git
```

## Features

### routes

Se incluye una ruta de ejemplo y un test "Hola mundo".

En caso de no requerir rutas:
 
- Eliminar el archivo `src/routes.php`
- Quitar las referencias de `src/PhpLibraryBoilerplateServiceProvider.php`.


### config

Se incluye un archivo de configuración y algunas configuraciones de ejemplo.

En caso de no requerir archivo de configuración:

- Eliminar el archivo `config/php-library-boilerplate.php`
- Quitar las referencias de `src/PhpLibraryBoilerplateServiceProvider.php`.


Reemplazar masivamente los strings:

- `php-library-boilerplate`: `example-project`
- `PhpLibraryBoilerplate`: `ExampleProject`

Instalar dependencias y probar que todo funcione bien.

```shell
composer update
vendor/bin/pest
```


## Tareas siguientes

- Comprobar licencia: Por defecto utiliza MIT.

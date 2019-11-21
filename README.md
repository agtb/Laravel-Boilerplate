# Laravel boilerplate

Useful and reusable configuration for Laravel development.

Including:

## [Bash / command line aliases .aliases](.aliases)

* Convenient timesaving for frequently used commands e.g. Artisan, Composer, PHPUnit, Vagrant. 
* To use: copy the aliases you like into `~/.bash_aliases` or simply `source .aliases`

To include the function output in a command use `$(functionName)`

e.g.

Create a Git tag 
```bash
git tag $(dt)
```

## [PHP CodeSniffer config phpcs.xml](phpcs.xml) optimized for Laravel dev

* [PSR-12](https://www.php-fig.org/psr/psr-12/)
* Excludes the obvious e.g. Blade files, vendor dirs
* Tests: allow underscores in method names e.g. given_when_then
* Database migrations and seeders: allow no namespaces (can break migrations, seeding)

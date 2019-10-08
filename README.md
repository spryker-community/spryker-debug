Spryker Debug
=============

[![Build Status](https://travis-ci.org/inviqa/spryker-debug.svg?branch=master)](https://travis-ci.org/inviqa/spryker-debug)

Collection of debug and development tools for Spryker:

Installation
------------

Require the package with composer:

```
$ composer require inviqa/spryker-debug
```

Add the `Inviqa` namespace to your `config/Shared/config_default.php` file:

```php
$config[KernelConstants::PROJECT_NAMESPACES] = [
    'Pyz',
    'Inviqa',
];
```

Each feature needs to be enabled individually. Instructions provided in the
documentation.

Features
--------

Follow the link for documentation:

### Console Commands

- [Config Dump](doc/config_dump.md): Introspect configuration.
- [Route Debug](doc/route_debug.md): Inspect routes from Yves
- [Database Shell](doc/database_shell.md): Launch a postgres shell.
- [Redis Shell](doc/redis_shell.md): Launch a Redis shell.
- [Queue Overview](doc/queue_overview.md): Show queue statuses.

### Integrations

- [Twig Var Dumper](doc/twig_var_dumper.md): `{{ dump() }}` without destroying the world.
- [Var Dump Server](doc/var_dump_server.md): Bring `dump()` messages to
  the CLI.

Developing
----------

Run the tests:

```
composer integrate
```

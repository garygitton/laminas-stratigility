# Installation and Requirements

Install this library using composer:

```console
$ composer require laminas/laminas-diactoros laminas/laminas-stratigility
```

Stratigility has the following dependencies (which are managed by Composer):

- `psr/http-message`, which provides the interfaces specified in [PSR-7](http://www.php-fig.org/psr/psr-7),
  and type-hinted against in this package. In order to use Stratigility, you will need an
  implementation of PSR-7; one such package is
  [laminas/laminas-diactoros](https://github.com/laminas/laminas-diactoros).

- `laminas/laminas-escaper`, used by the `FinalHandler` for escaping error messages prior to
  passing them to the response.

You can provide your own request and response implementations if desired as long as they implement
the PSR-7 HTTP message interfaces.
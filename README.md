# Initialize

```sh
$ phpenv local 7.1.29
$ composer install
$ php vendor/bin/codecept bootstrap
```

# Configurations

```sh
$ vim tests/acceptance.suite.yml
```

# Download ChromeDriver

```sh
$ curl -O https://chromedriver.storage.googleapis.com/77.0.3865.10/chromedriver_mac64.zip
$ unzip chromedriver_mac64.zip
```

# Download geckodriver

```
$ curl -O https://github.com/mozilla/geckodriver/releases/download/v0.24.0/geckodriver-v0.24.0-macos.tar.gz
$ tar zxvf geckodriver-v0.24.0-macos.tar.gz
```

# Write Acceptance Tests

Tests should be placed in `tests/acceptance` directory.

# Run ChromeDriver

```
$ ./chromedriver --url-base=/
```
# Run geckodriver

```
$ ./geckodriver -v --port 9515
```

# Run the Tests

```sh
$ vendor/bin/codecept run --debug
```

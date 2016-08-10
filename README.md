# Freegeoip service in PHP

DO NOT use this in production

Installation
----

```sh
composer require alxhotel/freegeoip-php
```

Usage
----

```php
<?php
// Create freegeoip object
$freegeoip = new Freegeoip();

// Get client
$clent = $freegeoip->client;

// Test IP
$output = $client->lookup("8.8.8.8");

// Print output
print_r($output);

/*
Array
(
    [ip] => 8.8.8.8
    [country_code] => US
    [country_name] => United States
    [region_code] => CA
    [region_name] => California
    [city] => Mountain View
    [zip_code] => 94035
    [time_zone] => America/Los_Angeles
    [latitude] => 37.386
    [longitude] => -122.0838
    [metro_code] => 807
)
*/

```

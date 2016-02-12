# PHP proxy

## Intro

This is simple php code/class which proxies REST api calls from local domain to remote api server.

## Install

Git clone then

```
cd php-proxy
cp dist.config.php config.php
```

and update configuration settings in `config.php` server params.

## Usage

In your JS client set all urls to be:

```
http://your-server-path/proxy.php?path=/api_path
```

## Example

Let's say you have api endpoint

```
http://api.example.com/entities
```

in your `config.php` set

```
return [
    'destination_url' => 'http://api.example.com'
];
```

let's say your domain is `www.example.com`, and then link to your endpoint is

```
http://www.example.com?path=/entities
```


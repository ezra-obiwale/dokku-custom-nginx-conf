# dokku custom-nginx-conf

This plugin implements [http://dokku.viewdocs.io/dokku/configuration/nginx/#customizing-via-configuration-files-included-by-the-default-tem](http://dokku.viewdocs.io/dokku/configuration/nginx/#customizing-via-configuration-files-included-by-the-default-tem)
but makes it so you don't need to get into the server to set it.

## Requirements

- dokku v0.20.x+
- docker 19.03.+

## Installation

```bash
sudo dokku plugin:install https://github.com/ezra-obiwale/dokku-custom-nginx-conf.git custom-nginx-conf
```

## Usage

1. Create an `custom-nginx.conf` file in the root directory of your application.
2. That's all.

The `custom-nginx.conf` file is copied to your apps`nginx.conf.d/` directory when
you push to the server.

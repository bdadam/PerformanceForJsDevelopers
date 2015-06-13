## HTML kann man ja auch minifizieren

- unnötige Apostrophe entfernen
- unnötiges Whitespace entfernen
- usw.

--

# Tools

`htmlmin` oder `grunt-contrib-htmlmin`

`npm i -g htmlmin`

--

```HTML
<!doctype html>
<html>
    <head>
        <meta charset="utf-8">
        <meta name="description" content="Test description">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <title>Test title</title>
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>
        <p>
            Lorem ipsum dolor sit amet.
        </p>
        <p>
            Lorem ipsum dolor sit amet.
        </p>
    </body>
</html>
```

--

```HTML
<!doctype html><html><head><meta charset="utf-8" /><meta name="description" content="Test description" /><meta name="viewport" content="width=device-width, initial-scale=1" /><title>Test title</title><link rel="stylesheet" href="css/style.css" /></head><body><p>
            Lorem ipsum dolor sit amet.
        </p><p>
            Lorem ipsum dolor sit amet.
        </p></body></html>
```

--

# 16% Ersparnis bei diesem Beispiel

--

# Im Server

- `ngx_pagespeed` für NginX
- `mod_page_speed` für Apache vom Google
### HTML

<img data-src="assets/346483297_c4cb93ab4e_o.jpg">
<div class="attribution">[flickr/jesper](https://www.flickr.com/photos/jesper/346483297/)</div>

--

# Static Webseiten

- Sind schnell
- Können fast überall gehostet werden
- Deployment ist nur Kopieren von Files

--

## Tools

- assemble.io
- metalsmith.io

--

## Workflow

- Templates werden unterstützt
- Man kann in Markdown schreiben
- HTML wird am Entwicklerrechner generiert und getestet

Note:
Handlebars

--

#### Nachteile

- Nicht so flexibel
- Es gibt kein Web Interface

--

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

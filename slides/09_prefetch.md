<!-- .slide: data-background="assets/7515152254_020a9851b4_k.jpg" -->
<div class="attribution">[flickr/lauralewis23](https://www.flickr.com/photos/lauralewis23/7515152254/)</div>

## Fake it till you make it!

--

# Prefetch

```html
IE9+, Firefox, Chrome, Safari, ...
<link rel="prefetch" href="/images/big.jpg">

IE10+, Firefox, Chrome, Safari, ...
<link rel="dns-prefetch" href="http://www.example.com/">

// Chrome only
<link rel="subresource" href="/my-javascript-file.js">
```

--

# Prerender

```html
<link rel="prerender" href="http://www.example.com/">
```

Nur Chrome und IE11

~~Firefox, Safari~~

--

# JavaScript FTW

```JavaScript
function prefetch(url) {
    var link = document.createElement('link');
    link.rel = 'prefetch';
    link.href = url;
    document.head.appendChild(link);
}

prefetch('/images/big.jpg');
```

--

```JavaScript
var nextPageLink = document.querySelector('#nextPageLink');
nextPageLink.addEventListener('mouseover', function() {
    prefetch(nextPageLink.href);
});

```

--

# Perceived Performance

--

# instantlick.io

- Lädt die nächste Seite schon beim `mouseover` oder `touchstart`
- Verzögerung zwischen `hover` und `click` ist ca. 200-300ms
- Umwandelt Webseiten nach "Single Page Apps" mit wenig Kosten

--

# SPFJS

- Partielles Pageload, wie auf Youtube
- Macht SPAs aus konventionellen Webseiten
- Bietet Prefetch-Support an

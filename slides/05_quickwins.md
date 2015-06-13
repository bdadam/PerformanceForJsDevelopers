# Quickwins

- gut automatisierbar
- oder nur Konfigurationssache

--

# Keine HTTP-Redirects

- Viel zu viel Overhead
- Vor allem auf mobilen Geräten

--

# Weniger DNS-Lookups

- Möglicherweise nur eine Domain benutzen
- Domainsharding braucht man nicht mehr, moderne Browser bauen 6 Connections per Origin paralell auf

--

<img data-src="assets/domain-shards.png">

> <footer>[Why Domain Sharding is Bad News for Mobile Performance and Users](http://www.mobify.com/blog/domain-sharding-bad-news-mobile-performance/)</footer>

--

# Gzip

<!-- .slide: data-background="assets/10.jpg" -->
<div class="attribution">Bild: [flickr/marcovdz](https://www.flickr.com/photos/marcovdz/4520986339/)</div>

--

# Caching

<!-- .slide: data-background="assets/6498619601_01056e83f7_o.jpg" -->
<div class="attribution">Bild: [flickr/kulturarvsprojektet](https://www.flickr.com/photos/kulturarvsprojektet/6498619601/)</div>

--

# Caching

- Ablaufdatum weit in die Zukunft setzen
- Beim zweiten Besuch muss der Browser viel weniger Daten runterladen
- Bei Änderungen URL auch ändern (Cachebusting)

<pre><code class="lang-html">&#x3C;script src=&#x22;main.js&#x22;&#x3E;&#x3C;/script&#x3E;
&#x3C;script src=&#x22;main.20150619.js&#x22;&#x3E;&#x3C;/script&#x3E;
&#x3C;script src=&#x22;main.js?20150619&#x22;&#x3E;&#x3C;/script&#x3E;
</code></pre>

--

# Bundling

statt mehreren Skript-Blöcken:
<pre><code class="lang-html">&#x3C;script src=&#x22;main.js?v145&#x22;&#x3E;&#x3C;/script&#x3E;
&#x3C;script src=&#x22;home.js?v67&#x22;&#x3E;&#x3C;/script&#x3E;
&#x3C;script src=&#x22;tracking.js?v41&#x22;&#x3E;&#x3C;/script&#x3E;
</code></pre>

nur einer:
<pre><code class="lang-html">&#x3C;script src=&#x22;main.js?v234&#x22;&#x3E;&#x3C;/script&#x3E;</code></pre>

--

# Bundling - Tools

- `cat main.js home.js tracking.js > all.js`
- grunt-contrib-concat
- ...

--

# Minifizieren

```js
(function() {
    var myLongVariableName = 123;
    var myEvenLongerVariableName = 256;

    function add(a, b) {
        return a + b;
    }

    var x = add(myLongVariableName, myEvenLongerVariableName);

    alert(x);
}());
```

```js
!function(){function n(n,r){return n+r}var r=123,t=256,u=n(r,t);alert(u)}();
```

--

# Minifizieren - Tools

- UglifyJS
- Google Clojure Compiler (braucht Java)
- ...

<!-- .slide: data-background="assets/5727299176_59317dbeb5_o.jpg" -->
<div class="attribution">Bild: [flickr/hikingartist](https://www.flickr.com/photos/hikingartist/5727299176/)</div>

--

# Vorgehensweise

- Requests schnell verarbeiten
- Anzahl der Requests reduzieren
- Grösse der Requests reduzieren
- Weniger DNS-Lookups
- Weniger bzw. keine HTTP-Redirects

--

<img src="assets/httparchive.org-2015-05-15/avg-bytes-per-page-by-content-type.png">

> <footer>[httparchive.org 15. Mai 2015](http://httparchive.org/interesting.php?a=All&l=May%2015%202015&s=Top1000)</footer>

--

<img src="assets/httparchive.org-2015-05-15/total-req-per-page.png">

> <footer>[httparchive.org 15. Mai 2015](http://httparchive.org/interesting.php?a=All&l=May%2015%202015&s=Top1000)</footer>

Note:
72% der Webseiten starten mehr als 50 Requests beim Laden!

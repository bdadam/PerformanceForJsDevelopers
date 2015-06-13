## Warum ist Web Performance wichtig?

--

# Wegen des Users

--

Responsezeit | UX
--|--
< 100ms | UI fühlt sich **instant** an
< 1 sec | Verzögerung wird wahrgenommen, der Benutzer wird aber noch nicht verloren
> 10 sec| Gedanken des Benutzers sind schon wo anders. Er fühlt sich nicht mehr im Griff zu haben, was der Computer (die Webseite) macht


> [Jakob Nielsen: Website Response Times](http://www.nngroup.com/articles/website-response-times/)

Note:
Nielsan hat die Studie zweimal durchgeführt, in 1997 und in 2010. Die Ergebnisse waren beide Mal sehr ähnlich.

--

### Genervte User sind verlorene User
<!-- .slide: data-background="assets/3645211083_4695ec1de4_o.jpg" -->
<div class="attribution">Photo: [flickr/Robert Couse-Baker](https://www.flickr.com/photos/29233640@N07/3645211083/)</div>

--

# Wegen dem Geld <!-- .element: class="dark-shadow" -->

<!-- .slide: data-background="assets/7027584837_77ac774e41_k.jpg" -->
<div class="attribution">Photo: [flickr/Tax Credits](https://www.flickr.com/photos/76657755@N04/7027584837/)</div>

--

### Beispiele
- Amazon (100ms Verbesserung = 1% mehr Revenue)
- Mozilla (-2,2 Sek. = 60M mehr Firefox Downloads)
- Yahoo (400ms Verbesserung = 9% mehr Traffic)
- Walmart (1 Sek. = 2% Conversion; 100ms = 1% mehr Revenue, SEO Vorteile)
- AOL, ShopZilla, Etsy, uvm.

--

# SEO-Effekt

<img data-src="assets/google-slow-label-mobile.png">

--

# Bandbreite<br>vs.<br>Latenz

Note:
man würde denken, dass eine fette Internetleitung alles löst, aber das ist eben nicht der Fall

--

<img data-src="assets/Latency_vs_bandwidth.png">
> <footer>[Ilya Grigorik](https://docs.google.com/presentation/d/1r7QXGYOLCh4fcUq0jDdDwKJWNqWK1o4xMtYpKZCJYjM/present#slide=id.g518e3c87f_2_0)</footer>

--

Lichtgeschwindigkeit = 300 000 km/s

***

Stadt | Entf. von München | RTT Vakuum | RTT Glasfaser*
--|--:|--:|--:
London    |  1.000km |   6ms |   9ms
New York  |  6.500km |  43ms |  65ms
Shanghai  |  9.000km |  60ms |  90ms
Sidney    | 16.000km | 106ms | 160ms

<p style="text-align: right;">\* Optimalwerte</p>

--

### Requests sind teuer

- TCP: Handshake, Slow-Start
- auf Desktop-Geräten ist Latenz eher das Problem
- auf Mobile sind sowohl Latenz als auch Bandbreite

--

<img src="assets/httparchive.org-2015-05-15/js-req-per-page.png">

> 68% der untersuchten Webseiten starten mehr als 10 JavaScript-Requests <footer>[httparchive.org 15. Mai 2015](http://httparchive.org/interesting.php?a=All&l=May%2015%202015&s=Top1000)</footer>

--

<img src="assets/httparchive.org-2015-05-15/js-transfer-size.png">

> 66% der untersuchten Webseiten laden mehr als 300KB JavaScript <footer>[httparchive.org 15. Mai 2015](http://httparchive.org/interesting.php?a=All&l=May%2015%202015&s=Top1000)</footer>

--

# Ziel

- Anzahl von Requests auf Minimum halten
- Übertragene Daten auf Minimum halten
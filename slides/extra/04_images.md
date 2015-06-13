# Bilder

--

## Bilder sind die grössten Assets im Web

<img src="assets/httparchive.org-2015-05-15/avg-bytes-per-page-by-content-type.png">

> <footer>[httparchive.org 15. Mai 2015](http://httparchive.org/interesting.php?a=All&l=May%2015%202015&s=Top1000)</footer>


--

<img src="assets/httparchive.org-2015-05-15/img-req-per-page.png">
> <footer>[httparchive.org 15. Mai 2015](http://httparchive.org/interesting.php?a=All&l=May%2015%202015&s=Top1000)</footer>
--

<img src="assets/httparchive.org-2015-05-15/img-transfer-size-per-page.png">
> <footer>[httparchive.org 15. Mai 2015](http://httparchive.org/interesting.php?a=All&l=May%2015%202015&s=Top1000)</footer>

--

# Imagemin

- Minifiziert die Bilder
- `npm i -g imagemin`
- CLI oder module
- grunt-contrib-imagemin

--

# SVG

- Markup Format
- Textbasiert
- Gut komprimierbar
- Animation, Styling

--

# grunticon

<img src="assets/grunticon.jpg">

- de facto Standard
- SVGs mit Fallbacks für ältere Browser

--

# Animierte GIFs

Können in MP4 konvertiert werden

Filegrösse reduziert sich extrem

`npm i videofy`

```JavaScript
videofy('input.gif', 'output.mp4', function(error) { /* ... */ });
```
# 3rd Party Content

--

#### aka.
# Cookie Monsters

<!-- .slide: data-background="assets/4592911516_4d8e73977c_o.jpg" -->
<div class="attribution">Bild: [flickr/x1brett](https://www.flickr.com/photos/x1brett/4592911516/)</div>

Note:
- 3rd party = cookie monster -> die setzen Cookies ohne Ende

--

Was sind die?
- Werbung (Google AdSense, Google DoubleClick)
- Tracking Pixels (Google Analytics, Piwik)
- Remarketing Pixels (Goodle AdWords Remarketing, Criteo)
- Comments (Disqus, Facebook)
- Social Network Plugins
- uvm.

--

<!-- .slide: data-background="assets/separation-concerns.png" -->
<div class="attribution">Bild: [SmashingMagazine](http://www.smashingmagazine.com/2014/09/08/improving-smashing-magazine-performance-case-study/)</div>

# Separation of Concerns

Note:
- SmashingMagazin hat keinen Nachteil bei async Ads gesehen

--

## Braucht man wirklich so viele Tools?

--

# Google Analytics

--

<img data-src="assets/psi-99.png">

--

## Google Analytics Measurement Protocol

```JS
// location.href === 'https://example.com/pageA'

new Image().src = '//www.google-analytics.com/collect?' +
'v=1&tid=UA-123456-1' + // tracker id
'&t=pageview' + // hit type
'&dp=%2FpageA' + // page url
'&cid=CLIENT_ID' + // some client id
'&z=' + +new Date();
```

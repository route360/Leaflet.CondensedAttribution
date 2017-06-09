# Leaflet.CondensedAttribution
An attribution plugin that makes long attributes visible on hover

Closed
![Alt text](attributes-closed.png?raw=true "Attributes Closed")

Open
![Alt text](attributes-open.png?raw=true "Attributes Open")

Branded - Closed
![Alt text](branded-closed.png?raw=true "Branded Closed")

Branded - Open
![Alt text](branded-open.png?raw=true "Branded Open")

## Demo
Refer to [index.html](index.html) or [see it live](https://route360.github.io/Leaflet.CondensedAttribution/).

## Features:
- condense overly-long attribution text
- add custom html to attribution emblem
- keep you map interface clean, without skimping on your attribution

## Installation
Include plugin files in project (after leaflet lib files)

```
<link rel="stylesheet" href="dist/leaflet-control-condended-attribution.css" />
<script type="text/javascript" src="dist/leaflet-control-condended-attribution.js"></script>
```

If you are not customizing it, you are good to go

If you want to customize, you have access to the options from Leaflet.Contol.Attribution, plus _emblem_, which sets the content for the un-expanded badge

```
var map = L.map('map', {
  condensedAttributionControl: false // don't include default, as we are setting options below
});

// set custom emblem and prefix
L.control.condensedAttribution({
  emblem: '<div class="emblem-wrap"><img src="https://www.route360.net/assets/images/logo_nav.png"/></div>',
  prefix: '<a href="https://www.route360.net/" title="Travel time analysis by Motion Intelligence">route360&deg;</a> | <a href="http://leafletjs.com" title="A JS library for interactive maps">Leaflet</a>'
}).addTo(map);
```
## Options:
- emblem - defines the content of the un-expanded attribution badge

## Details:
- Extends L.Control.Attribution, maintaining layer-based attribution.
- Defaults to show if plugin lib included in project, removing classic attribution
- works with leaflet 1.0 and prior

## [route360°](https://www.route360.net/)

The Route 360°-technology by Motion Intelligence provides a simple API for large geographic network analysis, route planning and visualization to power complex geo-applications. Our solutions can be integrated into your existing platform or can be build as a new application to suit your requirements. Let us help power your business with state-of-the art geo capabilities.

[Get your free API key](https://developers.route360.net/pricing/), and start mapping!

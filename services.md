---
layout: page
title: Services & Pricing
permalink: /services/
---

Getting a great-looking lawn doesn't have to be complicated or expensive. Here's exactly what I offer and what it costs.

## Services

<ul class="services-list">
  <li>
    <span class="service-emoji">🌿</span>
    <div class="service-details">
      <strong>Lawn Mowing</strong>
      <span>Mow, edge, and blow clippings off walkways — one tidy package.</span>
    </div>
    <div class="service-price">Starting at $[XX]</div>
  </li>
  <li>
    <span class="service-emoji">✂️</span>
    <div class="service-details">
      <strong>String Trimming / Edging</strong>
      <span>Clean up hard-to-reach spots along fences, garden beds, and curbs.</span>
    </div>
    <div class="service-price">$[XX]</div>
  </li>
  <li>
    <span class="service-emoji">💨</span>
    <div class="service-details">
      <strong>Blowing & Cleanup</strong>
      <span>Blow clippings and debris off driveways, sidewalks, and patios.</span>
    </div>
    <div class="service-price">$[XX]</div>
  </li>
  <li>
    <span class="service-emoji">🍂</span>
    <div class="service-details">
      <strong>Leaf Cleanup</strong>
      <span>Rake or blow leaves off your lawn and haul them to the curb.</span>
    </div>
    <div class="service-price">Starting at $[XX]</div>
  </li>
  <li>
    <span class="service-emoji">🌱</span>
    <div class="service-details">
      <strong>Spring / Fall Cleanup</strong>
      <span>Seasonal clear-out of debris, dead growth, and leaves to get your yard ready for the season.</span>
    </div>
    <div class="service-price">Starting at $[XX]</div>
  </li>
  <li>
    <span class="service-emoji">💩</span>
    <div class="service-details">
      <strong>Dog Poop Cleanup</strong>
      <span>We'll clear your yard of pet waste so it's clean, safe, and ready to enjoy.</span>
    </div>
    <div class="service-price">$[XX]</div>
  </li>
</ul>

---

## Pricing by Yard Size

<div class="pricing-table">
  <div class="pricing-card">
    <h3>Small Yard</h3>
    <div class="price">$[XX]</div>
    <ul>
      <li>Up to [X,XXX] sq ft</li>
      <li>Mow, edge, blow</li>
      <li>~[XX] minutes</li>
    </ul>
  </div>
  <div class="pricing-card featured">
    <h3>Medium Yard ⭐</h3>
    <div class="price">$[XX]</div>
    <ul>
      <li>[X,XXX]–[X,XXX] sq ft</li>
      <li>Mow, edge, blow</li>
      <li>~[XX] minutes</li>
    </ul>
  </div>
  <div class="pricing-card">
    <h3>Large Yard</h3>
    <div class="price">$[XX]</div>
    <ul>
      <li>[X,XXX]+ sq ft</li>
      <li>Mow, edge, blow</li>
      <li>~[XX] minutes</li>
    </ul>
  </div>
</div>

Not sure what size your yard is? No problem — just reach out and I'll give you a free quote.

<div style="text-align:center; margin-top: 30px;">
  <a href="/contact" class="btn btn-green">Get a Free Quote →</a>
</div>

---

## Service Area

I serve a **1-mile radius** around New Brighton, MN. Check the map below to see if I cover your neighborhood!

<div id="service-area-map"></div>

<script>
  function initMap() {
    var geocoder = new google.maps.Geocoder();
    geocoder.geocode({ address: '198 3rd Ave SE, New Brighton, MN 55112' }, function(results, status) {
      if (status === 'OK') {
        var center = results[0].geometry.location;
        var map = new google.maps.Map(document.getElementById('service-area-map'), {
          center: center,
          zoom: 13
        });
        new google.maps.Marker({
          map: map,
          position: center,
          title: 'Strong Mower HQ'
        });
        new google.maps.Circle({
          map: map,
          center: center,
          radius: 1609.34,
          fillColor: '#27AE60',
          fillOpacity: 0.15,
          strokeColor: '#27AE60',
          strokeOpacity: 0.9,
          strokeWeight: 2
        });
      }
    });
  }
</script>
<script async defer src="https://maps.googleapis.com/maps/api/js?key=%%GOOGLE_MAPS_API_KEY%%&callback=initMap"></script>

# Natural-Bridge-Valley


<html>

<head>
  <meta charset='utf-8' />
  <title>Display a map</title>
  <meta name='viewport' content='initial-scale=1,maximum-scale=1,user-scalable=no' />

  <script src='https://api.mapbox.com/mapbox-gl-js/v2.2.0/mapbox-gl.js'></script>
  <link href='https://api.mapbox.com/mapbox-gl-js/v2.2.0/mapbox-gl.css' rel='stylesheet' />

  <style>
    body {
      margin: 0;
      padding: 0;
    }

    #map {
      position: absolute;
      top: 0;
      bottom: 0;
      width: 100%;
    }
  </style>
</head>

<body>

  <div id='map'></div>

  <script>
    // 💡💡💡 Change this to your Token --------------------
    // ------------------------------------------------
    mapboxgl.accessToken = 'pk.eyJ1IjoiaG9nYW5mZWQiLCJhIjoiY2tvZndma3NuMG1mczJucHcwM2t0azZhNSJ9.hxCNV7pMHfEaK2T_xMekOA';
    // ------------------------------------------------
    // ------------------------------------------------

    var map = new mapboxgl.Map({
      container: 'map',

      // 💡💡💡 Change this to your style --------------------
      // ------------------------------------------------
      style: 'mapbox://styles/hoganfed/ckofxqh173rde17rxi4jw19yf',
      // ----------------------------------------------
      // ------------------------------------------------

      // 💡💡💡 Change to your location ----------------------
      // ------------------------------------------------
      zoom: 15.65,
      center: [-83.657662, 37.817418], 
      pitch: 85,
      bearing: 80
      // ------------------------------------------------
      // ----------------------------------------------

    });

    // Add geolocate control to the map.
    map.addControl(new mapboxgl.GeolocateControl({
      positionOptions: {
        enableHighAccuracy: true
      },
      trackUserLocation: true
    }));
  </script>

</body>

</html>
<html>

<head>
  <meta charset='utf-8' />
  <title>Display a tour</title>
  <meta name='viewport' content='initial-scale=1,maximum-scale=1,user-scalable=no' />

  <style>
    body {
      margin: 0;
      padding: 0;
    }

    section {
      width: 80%;
      margin: 0 auto;
    }

    h1, h2 {
      font-family: 'Work Sans', sans-serif;
    }
  </style>
</head>

<body>
  <section>
    <h2>Take a tour of Natural Bridge Valley</h2>

    <!-- 💡💡💡 paste embed code below -->

    <iframe title="Paint by Nature: Go See Trees" width="100%" height="800px" src="https://cesium.com/ion/stories/viewer/?id=395cc63a-ee79-4e9d-9266-10dd7ef2acf4" frameborder="0" allow="fullscreen" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
  
    </section>
</body>

</html>


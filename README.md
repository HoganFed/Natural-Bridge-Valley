# Natural-Bridge-Valley

Interactive Map

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
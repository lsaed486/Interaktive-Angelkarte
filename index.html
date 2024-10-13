<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Interaktive Angelkarte für den Kreis Pinneberg und Umgebung">
    <title>Interaktive Angelkarte Pinneberg</title>
    <link href="https://api.mapbox.com/mapbox-gl-js/v2.14.1/mapbox-gl.css" rel="stylesheet">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #3B5998;
            padding: 15px 0;
            color: white;
            text-align: center;
        }

        #map {
            width: 100%;
            height: 600px;
            margin-top: 20px;
        }

        .note-area {
            display: none;
        }

        .marker-input {
            margin-bottom: 10px;
        }

        .marker-color {
            width: 20px;
            height: 20px;
            display: inline-block;
            margin-right: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <header>
        <h1>Interaktive Angelkarte Pinneberg</h1>
        <p>Setze Marker für Gewässer:</p>
        <input type="text" id="marker-name" placeholder="Marker Name" class="marker-input">
        <div>
            <div class="marker-color" style="background-color: #0077BE;" data-color="#0077BE"></div>
            <div class="marker-color" style="background-color: #00BE77;" data-color="#00BE77"></div>
            <div class="marker-color" style="background-color: #BE7700;" data-color="#BE7700"></div>
        </div>
        <button id="set-marker">Marker Setzen</button>
    </header>

    <div id="map"></div>

    <script src="https://api.mapbox.com/mapbox-gl-js/v2.14.1/mapbox-gl.js"></script>
    <script>
        mapboxgl.accessToken = 'pk.eyJ1IjoibHNhZWQ0ODYiLCJhIjoiY20yNmxsNGZkMHhqbTJrc2o0dWg1OTRuYyJ9.iwQkgt5FL8kPQgpBozsakQ';

        var map = new mapboxgl.Map({
            container: 'map',
            style: 'mapbox://styles/mapbox/streets-v11',
            center: [9.7945, 53.6617],
            zoom: 9
        });

        let selectedColor = '#0077BE'; // Standardfarbe für Marker

        // Farbe auswählen
        document.querySelectorAll('.marker-color').forEach(colorDiv => {
            colorDiv.addEventListener('click', function() {
                selectedColor = this.getAttribute('data-color');
                document.querySelectorAll('.marker-color').forEach(div => div.style.border = '');
                this.style.border = '2px solid black';
            });
        });

        // Marker setzen
        document.getElementById('set-marker').addEventListener('click', function() {
            const name = document.getElementById('marker-name').value;
            if (!name) {
                alert('Bitte geben Sie einen Namen für den Marker ein.');
                return;
            }

            const markerEl = document.createElement('div');
            markerEl.className = 'marker';
            markerEl.style.backgroundColor = selectedColor;
            markerEl.style.width = '20px';
            markerEl.style.height = '20px';
            markerEl.style.borderRadius = '50%';

            const marker = new mapboxgl.Marker(markerEl)
                .setLngLat(map.getCenter())
                .setPopup(new mapboxgl.Popup({ offset: 25 })
                    .setHTML(`<h3>${name}</h3><p><a href="#" class="toggle-notes">Notizen hinzufügen</a></p><div class="note-area"><textarea rows="4" cols="20" placeholder="Notizen..."></textarea></div>`))
                .addTo(map);

            // Tooltip mit Marker-Namen
            markerEl.title = name;

            // Notizenbereich ein- und ausblenden
            markerEl.addEventListener('mouseenter', function() {
                marker.togglePopup();
            });

            markerEl.addEventListener('mouseleave', function() {
                marker.togglePopup();
            });

            // Notizenbereich
            markerEl.addEventListener('click', function() {
                const notesDiv = marker.getPopup().getDOMContent().querySelector('.note-area');
                notesDiv.style.display = notesDiv.style.display === 'block' ? 'none' : 'block';
            });
        });

    </script>

</body>
</html>

+++
# Any elements can be added in the body: https://sourcethemes.com/academic/docs/writing-markdown-latex/
# Add more sections by duplicating this file and customizing to your requirements.

widget = "base"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 120 # Order that this section will appear.


#title = "Database"
# subtitle = "Red Colaborativa en ecologia Microbiana de América Latina"

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "1"

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.

  # Background color.
   color = "Grey10"
  
  # Background gradient.
  #gradient_start = "DarkBlue"
  #gradient_end = "Cyan"
  
  # Background image.
  # image = "image.jpg"  # Name of image in `static/img/`.
  # image_darken = 0.6  # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.
  # image_size = "cover"  #  Options are `cover` (default), `contain`, or `actual` size.
  # image_position = "center"  # Options include `left`, `center` (default), or `right`.
  # image_parallax = true  # Use a fun parallax-like fixed background effect? true/false
  
  # Text color (true=light or false=dark).
  text_color_light = false

[design.spacing]
  # Customize the section spacing. Order is top, right, bottom, left.
  padding = ["20px", "0", "20px", "0"]

[advanced]
 # Custom CSS. 
 css_style = ""
 
 # CSS class.
 css_class = ""
+++

<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <title>Sedes de Gobierno - América del Sur</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- Leaflet -->
  <link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
  <script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>

  <style>
    body { margin: 0; padding: 0; }
    #map { height: 100vh; width: 100%; }

    .popup-img {
      width: 220px;
      border-radius: 8px;
      margin-bottom: 5px;
      box-shadow: 0 0 6px rgba(0,0,0,0.3);
    }

    .popup-content {
      text-align: center;
      font-family: sans-serif;
    }

    .popup-content a {
      text-decoration: none;
      color: #005fa3;
      font-weight: bold;
    }
  </style>
</head>

<body>
  <div id="map"></div>

  <script>
    const map = L.map('map').setView([-20, -60], 4);

    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      attribution: '&copy; OpenStreetMap contributors'
    }).addTo(map);

    // Lista das sedes de governo com imagens locais
    const edificios = [
      {
        nome: "Torre Ejecutiva - Uruguay",
        coords: [-34.9057, -56.1990],
        url: "https://www.presidencia.gub.uy/",
        imagem: "Edificio_Independencia.jpg"
      },
      {
        nome: "Casa Rosada - Argentina",
        coords: [-34.6081, -58.3702],
        url: "https://www.casarosada.gob.ar/",
        imagem: "Casa_Rosada.jpg"
      },
      {
        nome: "Palacio de La Moneda - Chile",
        coords: [-33.4429, -70.6531],
        url: "https://www.gob.cl/",
        imagem: "Palacio_de_La_Moneda.jpg"
      },
      {
        nome: "Palácio do Planalto - Brasil",
        coords: [-15.7993, -47.8619],
        url: "https://www.gov.br/planalto/",
        imagem: "Palácio_do_Planalto_GGFD8938.jpg"
      },
      {
        nome: "Casa de Nariño - Colômbia",
        coords: [4.5906, -74.0731],
        url: "https://m.www.gov.co/",
        imagem: "Casa_Narino.jpg"
      }
    ];

    edificios.forEach(edificio => {
      const marker = L.marker(edificio.coords).addTo(map);
      const popupHTML = `
        <div class="popup-content">
          <img class="popup-img" src="${edificio.imagem}" alt="${edificio.nome}">
          <div><strong>${edificio.nome}</strong></div>
          <a href="${edificio.url}" target="_blank">Visitar sitio oficial</a>
        </div>
      `;
      marker.bindPopup(popupHTML);
    });
  </script>
</body>
</html>
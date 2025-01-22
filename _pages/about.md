---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<p style="text-align: justify">

As a robotics engineer and recent Master's graduate from Northeastern University, I'm passionate about advancing visual SLAM systems for autonomous robots. My work at the Northeastern University Robust Autonomy Lab (NEURAL) focuses on developing computationally efficient Factor Graphs for Bundle Adjustment Problems and creating visual place recognition modules for multi-sensor navigation systems. I thrive on challenges that push the boundaries of visual perception in robotics.
<br>
My expertise extends beyond SLAM to various computer vision projects, including image restoration, stereo depth mapping, and 3D scene understanding. I'm particularly adept at applying deep learning models to solve complex perception challenges in robotics. My goal is to develop autonomous systems that can navigate complex, unlabeled environments safely and effectively. I'm always eager to collaborate on innovative projects that shape the future of robotics and computer vision.

</p>

Projects 
---------

<html>
<head>
  <style>
    .row {
      display: flex;
      flex-wrap: wrap;
      column-gap: 30px;
      justify-content: center; /* Center the columns horizontally */
    }
    .column {
      flex: 50%;
      padding: 20px;
      border: 1px solid grey; /* Add a border around each column */
      border-radius: 10px; /* Round the corners of the boxes */
      box-sizing: border-box; /* Include border and padding in element's total width and height */
      display: flex; /* Make the column a flex container */
      flex-direction: column; /* Stack the items vertically */
      align-items: center; /* Center the items horizontally */
    }
    .column img {
      width: 100%;
      height: auto;
      max-width: 300px;
      object-fit: cover;
      border-radius: 10px;
    }
    .column h2 {
      font-weight: bold;
      padding: 10px; /* Add padding around the title */
    }
    .column p {
      font-size: 14px; 
      text-align: justify;
      padding: 10px; /* Add padding around the description */
    }
  </style>
</head>
<body>
  <div class="row">
    {% for feature in site.data.features %}
      <div class="column">
        <img src="{{ feature.image_path }}" alt="{{ feature.alt }}">
        <h2> {{ feature.title }}  <a href="{{ feature.url }}"><code>Github</code></a></h2> <!-- Add feature.url in href -->
        <p>{{ feature.excerpt }}</p>
      </div>
    {% endfor %}
  </div>
</body>
</html>

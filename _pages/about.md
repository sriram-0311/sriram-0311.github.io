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

Hi! I'm Anush Sriram Ramesh, a passionate robotics engineer, Master's Graduate in Robotics from Northeastern University. I worked as a <b>Research Assistant</b> at <a href="https://neural.lab.northeastern.edu/">NEURAL</a> (Northeastern University Robust Autonomy Lab) headed by <a href="https://david-m-rosen.github.io/">Prof. David Rosen</a>, I’m focused on advancing visual SLAM systems to empower autonomous robots. My work involves building computationally efficient Factor Graphs for Bundle Adjustment Problems to enable large-scale mapping in multi-camera visual-inertial navigation systems. I’ve also developed a visual place recognition module using Bag of Words for long-term data association and loop closure detection in multi-sensor navigation systems.

Beyond my core research, I’m deeply excited about computer vision projects, ranging from image restoration and shadow decomposition to stereo depth mapping and 3D scene understanding. I thrive on exploring new ways to push the boundaries of visual perception, driving reliable autonomy in the real world. My ultimate goal is to develop autonomous systems that can safely and effectively navigate complex, unlabeled environments.

You can check out my work on GitHub or learn more about my research at NEURAL. I’m always eager to connect and collaborate—feel free to reach out! Let’s shape the future of robotics together!

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

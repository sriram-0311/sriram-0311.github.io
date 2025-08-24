---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<p style="text-align: justify; font-size: 14px;">

As a robotics engineer and Master's graduate from Northeastern University, I'm deeply passionate about advancing <b>perception systems for autonomous navigation</b> through cutting-edge research and industry collaboration. My expertise spans the full spectrum of perception technologies, from <b>traditional model-based approaches</b> like factor graph optimization and geometric SLAM to <b>deep learning model-free methods</b> including transformer architectures and end-to-end neural networks.

<br>

At Northeastern University's Robust Autonomy Lab (NEURAL) and through industry partnerships with <b>Toyota Research Institute</b>, I've developed production-ready perception systems that bridge the gap between academic research and real-world deployment. My work includes engineering <b>real-time multi-camera visual-inertial SLAM systems</b> with sub-10ms latency, implementing <b>DETR-based panoptic segmentation</b> for 360-degree scene understanding, and creating <b>robust sensor fusion architectures</b> that maintain performance across diverse environmental conditions.

<br>

I excel at leveraging both paradigms: employing <b>classical geometric methods</b> like Bundle Adjustment, factor graphs, and visual odometry for precise localization, while simultaneously harnessing <b>modern deep learning</b> through transformer architectures, temporal consistency networks, and multi-modal fusion for semantic scene understanding. This dual expertise allows me to architect comprehensive autonomous navigation systems that combine the reliability of model-based approaches with the adaptability of learned representations.

<br>

My ultimate goal is to develop <b>safety-critical perception systems</b> that enable autonomous vehicles to navigate complex, dynamic environments with human-level understanding and beyond-human reliability. I'm always eager to collaborate on innovative projects that push the boundaries of what's possible in autonomous navigation, whether through advancing SLAM algorithms, developing novel computer vision architectures, or creating production-scale perception pipelines for next-generation autonomous systems.

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

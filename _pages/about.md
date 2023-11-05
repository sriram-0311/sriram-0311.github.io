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

Hi! I'm Aryaman Patel, a robotics engineer pursuing my MS in Robotics at Northeastern University. I currently work as a <b>Research Assistant</b> at <a href="https://neural.lab.northeastern.edu/">NEURAL</a> (Northeastern University Robust Autonomy Lab) headed by <a href="https://david-m-rosen.github.io/">Prof. David Rosen</a> where my focus is on improving visual SLAM systems for autonomous robots.
<br>
I have dedicated significant effort to constructing <b>Factor Graphs for Bundle Adjustment</b> Problems, aiming to achieve computationally efficient mapping in large environments for a multi-camera-based visual-inertial navigation system. Additionally, I developed and implemented a <b>visual place recognition</b> module based on Bag of Words for long-term data association and loop closure detection in a multi-sensor navigation system.
<br>
Outside of my core research, I enjoy working on computer vision projects related to image restoration, intrinsic image decomposition, and 3D scene understanding. These include intrinsic image decomposition, shadow decomposition, stereo depth mapping, and more. I am passionate about pushing the boundaries of visual perception to enable reliable autonomy in the real world. You can view some of my work on <a href="https://github.com/aryaman-patel">GitHub</a> or learn more about my current robotics research at <a href="https://neural.lab.northeastern.edu/">NEURAL</a>. Please feel free to reach out to me!
<br>
I will complete my MS in Robotics in <b>2024</b> and continue pursuing my dream of developing autonomous systems that can operate safely and effectively in complex, unlabeled environments.

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

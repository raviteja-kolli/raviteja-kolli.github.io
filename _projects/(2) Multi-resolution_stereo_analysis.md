---
name: Multi-Resolution Stereo Analysis
tools: [Python, OpenCV]
image: https://raviteja-kolli.github.io/assets/project4.jpg
description: The Multi-Resolution Stereo Analysis project focuses on enhancing depth perception and disparity calculations for stereo image pairs through a combination of region-based and feature-based matching techniques. 
---

<br>
### Brief overview
<br>
This project aimed to implement a multi-resolution stereo analysis system using region-based and feature-based matching techniques to enhance depth perception and improve disparity calculations for stereo image pairs. The objective was to generate accurate disparity maps by integrating advanced algorithms with customizable user options.

### Software
* Python: Used for implementing the algorithms and processing images.

* OpenCV: Utilized for image manipulation, feature extraction, and performing various stereo analysis techniques.

**Methods Used:**
<br>
The multi-resolution stereo analysis project employed a combination of region-based and feature-based methods to achieve accurate disparity calculations. In the region-based analysis, user-defined templates and matching window sizes, which could be either square or rectangular, were used. Matching was performed along the x-direction using various metrics, including Sum of Absolute Differences (SAD), Sum of Squared Differences (SSD), and Normalized Cross-Correlation (NCC).
<br>
<img src="{{ site.url }}{{ site.baseurl }}/assets/SAD.png"/>
<br>

<br>
<img src="{{ site.url }}{{ site.baseurl }}/assets/NCC.png"/>
<br>
The feature-based analysis utilized the Harris Corner Detector for feature extraction and matching, with matching scores evaluated using SAD, SSD, and NCC to provide greater flexibility in the comparison process. To further enhance accuracy, the project implemented a validation process involving left-to-right and right-to-left matching, ensuring reliable disparity estimates. Additionally, gaps within the disparity maps were filled using adaptive neighborhood averaging, which allowed the use of larger window sizes for robust interpolation.

### Results and Future Scope

The project successfully generated accurate disparity maps for five different stereo pairs, demonstrating the effectiveness of the proposed methodology. By incorporating region-based analysis at the top resolution and feature-based matching at lower resolutions, the system achieved optimal results with enhanced depth perception and improved alignment accuracy across varying disparity levels.

Future improvements could involve integrating deep learning-based matching methods to enhance accuracy and robustness. Additionally, achieving real-time disparity calculations through parallel processing techniques could significantly improve the performance of the system. The developed model also has promising potential for deployment in various applications, including autonomous systems, 3D reconstruction, and real-time image processing tasks.

* Enhanced Features: Integration with deep learning-based matching methods for improved accuracy.

* Faster Algorithms: Achieving real-time disparity calculations using parallel processing techniques.

* Applications: Deploying the model for autonomous systems, 3D reconstruction, and other practical implementations.


### GitHub (code snippets)

Explore the details and code for the Multi-Resolution Stereo Analysis Project

<p class="text-center">
{% include elements/button.html link="https://github.com/raviteja-kolli/Multi-Resolution_Stereo_Analysis" text="GitHub" %}
</p>

---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/LDL
---

<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>LDL: Line Distance Functions for Panoramic Localization</title>

    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Encode+Sans:wght@300;400;500;600&family=Roboto+Mono&display=swap"
      rel="stylesheet"
    />

    <!-- Bulma -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css" />
    <link rel="stylesheet" href="{{ site.url }}{{ site.baseurl }}/css/styles.css" />
    <script src="{{ site.url }}{{ site.baseurl }}/js/bulma_toggle.js"></script>

    <!-- Font Awesome -->
    <script src="https://kit.fontawesome.com/5fd1dd8417.js" crossorigin="anonymous"></script>

    <!-- Academicons -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css" />
  </head>

  <body>
    <!-- logo img -->
    <nav class="navbar logo">
      <div class="navbar-brand logo">
        <a class="navbar-item logo" href="https://3d.snu.ac.kr/">
          <img src="{{ site.url }}{{ site.baseurl }}/images/3dv.png" />
        </a>
      </div>
    </nav>

    <!-- title / authors / icons -->
    <section class="hero">
      <div class="hero-body">
        <div class="container is-max-widescreen has-text-centered">
          <!-- title -->
          <h1 class="title is-size-1 is-size-2-mobile publication-title">
            <span style="color: #4287f5">LDL</span>: <span style="color: #4287f5">L</span>ine <span style="color: #4287f5">D</span>istance Functions <br/>for Panoramic <span style="color: #4287f5">L</span>ocalization
          </h1>

          <!-- authors -->
          <div class="container is-max-desktop has-text-centered">
            <div class="columns is-mobile is-centered is-gapless">
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://www.junhokim.xyz">Junho Kim</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="http://3d.snu.ac.kr/members">Changwoon Choi</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="http://3d.snu.ac.kr/members">Hojun Jang</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="http://3d.snu.ac.kr/members">Young Min Kim</a>
              </div>
            </div>
          </div>

          <div class="is-size-5-tablet publication-institute">
            <span class="author-block">Dept. of Electrical and Computer Engineering, Seoul National University</span>
          </div>

          <!-- icons -->
          <div class="is-size-5 link-blocks">
            <a class="button link-button is-rounded" href="{{ site.url }}{{ site.baseurl }}/assets/LDL/paper.pdf">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <a class="button link-button is-rounded" href="https://arxiv.org/abs/2308.13989">
              <span class="icon">
                <i class="ai ai-arxiv"></i>
              </span>
              <span>arXiv</span>
            </a>
            <a class="button link-button is-rounded" href="https://www.youtube.com/watch?v=cQ5l4rauNY0">
              <span class="icon">
                <i class="fa-brands fa-youtube"></i>
              </span>
              <span>Video</span>
            </a>
            <a class="button link-button is-rounded" href="https://github.com/82magnolia/panoramic-localization">
              <span class="icon">
                <i class="fab fa-github"></i>
              </span>
              <span>Code</span>
            </a>
          </div>
        </div>
      </div>
    </section>

    <!-- teasor -->
    <section class="hero">
      <div class="container is-max-desktop">
        <div class="hero-body">
          <img src="{{ site.url }}{{ site.baseurl }}/assets/LDL/thumbnail.gif" width="100%" style="display: block; margin: auto" />
          <h2 class="subtitle has-text-centered">
            LDL performs quick & robust localization by <b>matching the distribution of lines in 2D and 3D</b>.
          </h2>
        </div>
      </div>
    </section>

    <!-- content section with left-side subtitle, which is aligned to center -->
    <section class="section">
      <div class="container is-max-desktop">
        <!-- abstract -->
        <div class="columns">
          <div class="column is-one-fifth has-text-centered">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Abstract</h2>
          </div>
          <div class="column has-text-justified">
            <p class="content">
              We introduce LDL, a fast and robust algorithm that
              localizes a panorama to a 3D map using line segments.
              LDL focuses on the sparse structural information of lines
              in the scene, which is robust to illumination changes and
              can potentially enable efficient computation. While previous line-based localization approaches tend to sacrifice
              accuracy or computation time, our method effectively observes the holistic distribution of lines within panoramic
              images and 3D maps. Specifically, LDL matches the distribution of lines with 2D and 3D line distance functions,
              which are further decomposed along principal directions of
              lines to increase the expressiveness. The distance functions
              provide coarse pose estimates by comparing the distributional information, where the poses are further optimized
              using conventional local feature matching. As our pipeline
              solely leverages line geometry and local features, it does not
              require costly additional training of line-specific features
              or correspondence matching. Nevertheless, our method
              demonstrates robust performance on challenging scenarios including object layout changes, illumination shifts, and
              large-scale scenes, while exhibiting fast pose search terminating within a matter of milliseconds. We thus expect our
              method to serve as a practical solution for line-based localization, and complement the well-established point-based
              paradigm. The code for LDL is available through the following link: <a href="https://github.com/82magnolia/panoramic-localization">https://github.com/82magnolia/panoramic-localization</a>.
            </p>
          </div>
        </div>

        <!-- video -->
        <div class="columns">
          <div class="column is-one-fifth has-text-centered">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Video</h2>
          </div>
          <div class="column">
            <div class="publication-video">
              <iframe
                src="https://www.youtube.com/embed/cQ5l4rauNY0?si=KexQ7mQW2VMcqOub"
                allow="autoplay; encrypted-media"
                allowfullscreen="true"
              ></iframe>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- content section with left-side subtitle -->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="columns">
          <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">
              Task Overview
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/LDL/overview.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              LDL is a localization algorithm that takes a panorama image as input and finds the camera pose with respect to a 3D point cloud map. 
              LDL <b>exploits line information during localization</b> to further reduce the map size and attain robustness against 2D-3D domain gaps or illumination changes.
              This is in contrast to many prior methods that use photometric cues, which are susceptible to the aforementioned issues.              
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Content section with left-side subtitle -->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="columns">
          <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Method Overview</h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/LDL/method.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              LDL performs localization through a three step process.
              First, LDL extracts lines, principal directions, and local feature descriptors from the panorama and point cloud.
              Then, LDL performs coarse pose search using novel line descriptors called line distance functions.
              As the final step, LDL applies local feature matching between the panorama and selected poses within the map to obtain the refined pose.              
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Content section with left-side subtitle -->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="columns">
          <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">
              Line Distance Functions Overview
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/LDL/line_distance_function.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              During coarse pose search, we exploit <b>line distance functions in 2D and 3D</b>.
              The distance functions are designed to capture the holistic distribution of lines.
              First, 2D line distance functions are defined as the spherical distance to the nearest line segment.
              3D line distance functions are similarly defined for pool of poses within the map.
              Specifically, for each pose we first project the 3D line segments onto the sphere and compute the line distance function values.                
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Content section with left-side subtitle -->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="columns">
          <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">
              Line Distance Function Decomposition
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/LDL/decomposition.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              We further <b>decompose line distance functions using principal directions</b>.
              Instead of defining a single distance function using all visible lines, we define three line distance functions for each set of lines parallel to the principal directions.
              The decomposed line distance functions are finally compared using a robust cost function.
              Here the cost function is defined for each rotation and translation within the map, and compares the decomposed distance function values for uniformly sampled points on the sphere.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="section">
        <div class="container is-max-desktop">
        <div class="columns">
            <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">
                Localization Performance Analysis
            </h2>
            </div>
            <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/LDL/eval_samples.png" width="100%" style="display: block; margin: auto" />
            We evaluate LDL on Stanford2D-3D-S and OmniScenes, which are common datasets used for evaluating panoramic localization.
            As shown above, numerous scenes in these datasets contain repetitive structures and noisy lines.

            <img src="{{ site.url }}{{ site.baseurl }}/assets/LDL/exp_results.png" width="80%" style="display: block; margin: auto" />

            The figure on the left shows the translation and rotation recall curves for LDL and a conventional learning-based pose search method called NetVLAD.
            LDL shows performance on a par with the learning-based method, while maintaining an order-of-magnitude shorter time.            

            </div>
        </div>
        </div>
    </section>

    <section class="section">
    <div class="container is-max-desktop">
        <div class="columns">
        <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">
            Potential for Privacy Protection
            </h2>
        </div>
        <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/LDL/privacy_line.png" width="80%" style="display: block; margin: auto" />

            We find that a small modification our method can offer light-weight privacy protection in client-server localization scenarios.
            By changing LDL to only exploit local features near lines during refinement, we can prevent privacy breaches such as feature inversion attacks which aim to reveal the original image content from local feature information.

            <img src="{{ site.url }}{{ site.baseurl }}/assets/LDL/privacy_curve.png" width="80%" style="display: block; margin: auto" />

            Here we plot the image error metrics of feature inversion attacks against the original image along with the localization accuracy using various line-based filtering threshold values.
            While the discrepancy values increase largely, the localization accuracy remains relatively constant.

        </div>
        </div>
    </div>
    </section>

    <!-- BibTex sectoion -->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="column is-full-width is-centered has-text-centered">
          <h2 class="subtitle is-size-3 has-text-weight-medium publication-keywords">BibTeX</h2>
        </div>
        <div class="box bibtex-box">
          <pre>
@InProceedings{Kim_2023_ICCV,
  author    = {Kim, Junho and Choi, Changwoon and Jang, Hojun and Kim, Young Min},
  title     = {LDL: Line Distance Functions for Panoramic Localization},
  booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
  month     = {October},
  year      = {2023},
  pages     = {17882-17892}
}          
        </pre>
        </div>
      </div>
    </section>

    <!-- Footer section -->
    <footer class="footer" style="padding-top: 1rem">
      <!-- navigation -->
      <a role="button" class="navbar-burger" data-target="moreResearch" aria-label="menu" aria-expanded="false">
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
      <div class="navbar-menu" id="moreResearch">
        <div class="navbar-start" style="flex-grow: 1; justify-content: center">
          <div class="block is-flex" style="margin-bottom: 0px">
            <a class="navbar-item" href="https://www.junhokim.xyz">
              <span class="icon">
                <i class="fas fa-home"></i>
              </span>
            </a>
            <a class="navbar-item" href="https://github.com/82magnolia">
              <span class="icon">
                <i class="fab fa-github"></i>
              </span>
            </a>
          </div>
          <div class="navbar-item has-dropdown has-dropdown-up is-hoverable">
            <a class="navbar-link">More Research</a>

            <div class="navbar-dropdown is-right">
              <a class="navbar-item" href="https://82magnolia.github.io/piccolo/">
                PICCOLO: Point Cloud-Centric Omnidirectional Localization
              </a>
              <a class="navbar-item" href="https://82magnolia.github.io/cpo/">
                CPO: Change Robust Panorama to Point Cloud Localization
              </a>
              <a class="navbar-item" href="https://82magnolia.github.io/event_localization/">
                Event-Based Visual Localization
              </a>
              <a
                class="navbar-item"
                href="https://openaccess.thecvf.com/content/WACV2023/html/Hwang_Ev-NeRF_Event_Based_Neural_Radiance_Field_WACV_2023_paper.html"
              >
                Event-Based Neural Radiance Fields
              </a>
            </div>
          </div>
        </div>
      </div>

      <!-- license -->
      <div class="content has-text-centered" style="margin-top: 1.6rem">
        <p>
          This website is licensed under a
          <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"
            >Creative Commons Attribution-ShareAlike 4.0 International License</a
          >
        </p>
      </div>
    </footer>
  </body>
</html>

---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/CPO
---

<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>CPO: Change Robust Panorama to Point Cloud Localization</title>

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
            <span style="color: #4287f5">CPO</span>: <span style="color: #4287f5">C</span>hange Robust <span style="color: #4287f5">P</span>anorama to <br>Point Cloud L<span style="color: #4287f5">o</span>calization
          </h1>
          <!-- authors -->
          <div class="container is-max-desktop has-text-centered">
            <div class="columns is-mobile is-centered is-gapless">
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://www.junhokim.xyz">Junho Kim</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://hojunjang17.github.io">Hojun Jang</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://www.changwoon.info">Changwoon Choi</a>
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
            <a class="button link-button is-rounded" href="{{ site.url }}{{ site.baseurl }}/assets/CPO/paper.pdf">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <a class="button link-button is-rounded" href="https://arxiv.org/abs/2207.05317">
              <span class="icon">
                <i class="ai ai-arxiv"></i>
              </span>
              <span>arXiv</span>
            </a>
            <a class="button link-button is-rounded" href="https://www.youtube.com/watch?v=V6XjHL5q0_Y">
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
          <img src="{{ site.url }}{{ site.baseurl }}/assets/CPO/qual_results.png" width="100%" style="display: block; margin: auto" />
          <h2 class="subtitle has-text-centered">
            CPO is a localization algorithm that operates by <b>matching color distributions</b> in 2D and 3D.
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
              We present CPO, a fast and robust algorithm that localizes a 2D panorama with respect to a 3D point cloud of a scene possibly containing changes. 
              To robustly handle scene changes, our approach deviates from conventional feature point matching, and focuses on the spatial context provided from panorama images.
              Specifically, we propose efficient color histogram generation and subsequent robust localization using score maps. 
              By utilizing the unique equivariance of spherical projections, we propose very fast color histogram generation for a large number of camera poses without explicitly rendering images for all candidate poses. 
              We accumulate the regional consistency of the panorama and point cloud as 2D/3D score maps, and use them to weigh the input color values to further increase robustness.
              The weighted color distribution quickly finds good initial poses and achieves stable convergence for gradient-based optimization. 
              CPO is lightweight and achieves effective localization in all tested scenarios, showing stable performance despite scene changes, repetitive structures, or featureless regions, which are typical challenges for visual localization with perspective cameras.
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
                src="https://www.youtube.com/embed/V6XjHL5q0_Y?si=mkS9IrG3UbSSaBKe"
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
              Challenges in Panoramic Localization
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/CPO/motivation.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              CPO is a localization algorithm that takes a panorama image and colored point cloud as input and finds the camera pose.
              Panorama images are beneficial for localization as the full 360-degree view provides the holistic scene context with less ambiguity.
              However, drastic scene changes can make localization challenging, as illustrated in the right.
              The goal of CPO is to perform robust localization amidst such scene changes.
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
            <img src="{{ site.url }}{{ site.baseurl }}/assets/CPO/overview.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              Given a query image and point cloud, CPO first creates 2D, 3D score maps that reflect regional color consistencies and attenuate regions that possibly contain scene changes.
              Using the score maps, CPO first selects promising candidate poses which are further refined with gradient descent optimization.              
            </p>
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
              2D Score Map Generation
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/CPO/2d_score_map.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              2D score maps assign higher scores to <b>image regions that are consistent with the point cloud color</b>.
              To create 2D score maps, synthetic views are first rendered at various locations in the point cloud.
              Then, intersections are computed between the patch-wise color histograms of the synthetic views and the query image.
              Finally, for each patch in the 2D score map, the maximum histogram intersection is stored.              
            </p>
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
              3D Score Map Generation
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/CPO/3d_score_map.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              3D score maps assign higher scores to <b>point cloud regions that have consistent colors with the query image</b>.
              To build 3D score maps, we re-use the patch-wise histogram intersections computed between the query image and synthetic views.
              For each synthetic view, we back-project the histogram intersection values to the point cloud, and average the back-projected histogram intersections.              
            </p>
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
              Localization Step 1: Candidate Pose Selection
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/CPO/candidate_pose_selection.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              CPO leverages the 2D score map for candidate pose selection.
              Given a pool of translations and rotations, CPO renders a synthetic view for each pose and computes the patch-wise color histograms.
              The histograms are compared against the query image through histogram intersection weighted with 2D score maps.
              Finally, the top-k poses with the largest intersection values are selected for refinement.
            </p>
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
              Localization Step 2: Pose Refinement
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/CPO/pose_refinement.png" width="90%" style="display: block; margin: auto" />
            <p class="content">
              CPO uses the 3D score map with sampling loss minimization for pose refinement.
              Sampling loss is defined as the color difference between each 3D point’s color and its projected location’s sampled color.
              Here, the 3D score map is applied to weigh the color difference of each point.
              On the right, we show the optimization trajectories of the candidate poses.
              The candidate pose with the smallest sampling loss is chosen after optimization.              
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
              2D and 3D Score Map Visualization
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/CPO/score_map_vis.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              Here we show visualizations of 2D, 3D score maps.
              On the left, new furniture and a moving person are introduced since the 3D scan, which are all attenuated by the 2D score map.
              On the right, we display the 3D score map, where the map places smaller values on regions near chairs and the blue carpet which are not present in the query image.              
            </p>
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
@InProceedings{Kim_2022_ECCV,
    author    = {Kim, Junho and Jang, Hojun and Choi, Changwoon and Kim, Young Min},
    title     = {CPO: Change Robust Panorama to Point Cloud Localization},
    booktitle = {Proceedings of the European Conference on Computer Vision (ECCV)},
    month     = {October},
    year      = {2022},
    pages     = {176-192},
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
              <a class="navbar-item" href="https://82magnolia.github.io/event_localization/">
                Event-Based Visual Localization
              </a>
              <a class="navbar-item" href="https://3d.snu.ac.kr/publications/PICCOLO">
                PICCOLO: Point Cloud-Centric Omnidirectional Localization
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

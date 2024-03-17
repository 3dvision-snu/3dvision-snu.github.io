---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/NFL
---

<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>NFL: Normal Field Learning for 6-DoF Grasping of Transparent Objects</title>

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
            NFL: Normal Field Learning for <br>6-DoF Grasping of Transparent Objects
          </h1>

          <!-- authors -->
          <div class="container is-max-desktop has-text-centered">
            <div class="columns is-mobile is-centered is-gapless">
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://twjhlee.github.io/">Junho Lee</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="http://3d.snu.ac.kr/members">Sangmin Kim</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://www.gabe-yhlee.com">Yonghyeon Lee</a>
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
            <a class="button link-button is-rounded" href="{{ site.url }}{{ site.baseurl }}/assets/NFL/NFL_RAL_final.pdf">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <a class="button link-button is-rounded" href="https://www.youtube.com/watch?v=b92CTDKeEk8&ab_channel=3DVisionLabattheSeoulNationalUniversity">
              <span class="icon">
                <i class="fa-brands fa-youtube"></i>
              </span>
              <span>Video</span>
            </a>
            <a class="button link-button is-rounded" href="https://github.com/twjhlee/Normal-Field-Learning">
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
          <img src="{{ site.url }}{{ site.baseurl }}/assets/NFL/projectpage_thumbnail.png" width="100%" style="display: block; margin: 0px -10px -30px -15px" />
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
                We present Normal Field Learning (NFL), a robust
                yet practical solution to perceive 3D layouts of transparent
                objects and grasp them quickly. Conventional input modalities for
                vision-based grasping do not provide sufficient information for
                transparent objects. However, with the recent advance on datasets
                and algorithms for transparent objects, we can at least obtain
                noisy estimates of normals and masks for various real-world
                conditions. Instead of directly using the RGB images, we propose
                to use the estimates to train a neural volume, which serves as an
                intermediate representation ignorant of challenging appearance
                variations. We formulate the training objective to account for in-
                herent uncertainty in individual estimation, and together with the
                volumetric aggregation, we can reliably extract useful geometric
                information for grasping. Our neural volume deploys a voxel-
                grid based representation, motivated by acceleration techniques
                of neural radiance fields. However, we directly store the normal
                and density values in the grid cells instead of latent features. Our
                modification allows direct access to the geometric values without
                additional inference or volume rendering, further enhancing the
                efficiency. Our results show over 85% success rates in grasping
                in cluttered scenes with only 40 seconds of training time.
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
                src="https://www.youtube.com/embed/b92CTDKeEk8?si=iSGa_AB8JxwacHgZ"
                allow="autoplay; encrypted-media"
                allowfullscreen="true"
                style="display: block; margin: 10px 0px 10px 0px"
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
              Method Overview
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/NFL/fig2_overview_v2.png" width="100%" style="display: block; margin: -0px 0px 10px 0px" />
            <p class="content">
            The inputs for probabilistic normal field learning are the pixel-wise estimation of surface normal modeled as von Mises-Fisher distribution and estimated object mask modeled as a Bernoulli distribution.
            The output is a 3D normal field where each point is mapped to a normal vector n and density σ.
            From the normal field, we sample reliable grasps, among which we select one that can induce trajectory without collision(green grasps).
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
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Qualitative Results</h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/NFL/fig5_qual_results_graspnerf.png" width="100%" style="display: block; margin: -20px 10px 10px 10px" />
            <p class="content">
                Qualitative results across various scenes. We visualize the geometric
                representations that different methods use for grasping (normal field for ours,
                depth image for baselines). Our method stably creates normal fields for real
                world, Dex-NeRF, and blender scenes. GraspNeRF finds the ground, but
                occasionally fails to reconstruct the geometry.
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
                <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Grasp Setting</h2>
            </div>
            <div class="column has-text-justified">
                <img src="{{ site.url }}{{ site.baseurl }}/assets/NFL/fig6_grasp_setting.png" width="100%" style="display: block; margin: 0px 0px 10px 0px" />
                <p class="content">
                   We experiment in a real world setup with glass textured objects.
                   For capturing images, we use a RealSense d435i camera mounted on a Franka Emika Panda robot arm. 
                   Capturing takes up to 1 second per image.
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
                <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Geometric Evaluation</h2>
            </div>
            <div class="column has-text-justified">
                <img src="{{ site.url }}{{ site.baseurl }}/assets/NFL/fig3_qual_results_blender.png" width="100%" style="display: block; margin: -40px 0px 0px 0px" />
                <p class="content">
                    Above image shows the quality of reconstructed geometry on our blender dataset.
                    The top row depicts the rendered depth and the bottom row the corresponding error map(Blue: low error).
                    NFL outperforms the rest.
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
                <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Ablation on input modality</h2>
            </div>
            <div class="column has-text-justified">
                <img src="{{ site.url }}{{ site.baseurl }}/assets/NFL/fig4_input_modality.png" width="100%" style="display: block; margin: -40px 0px 10px 0px" />
                <p class="content">
                    Above image shows the error maps on depth per input modality(Blue: low error).
                    For transparent glass textured objects, the mixture of normal and mask produces the best result.
                    Especially, RGB inputs fail for both DVGO and NeRF.
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
          <pre>@ARTICLE{10328050,
  author={Lee, Junho and Kim, Sang Min and Lee, Yonghyeon and Kim, Young Min},
  journal={IEEE Robotics and Automation Letters}, 
  title={NFL: Normal Field Learning for 6-DoF Grasping of Transparent Objects}, 
  year={2024},
  volume={9},
  number={1},
  pages={819-826},
  keywords={Grasping;Three-dimensional displays;Estimation;Training;Rendering (computer graphics);Cameras;Uncertainty;Deep Learning for Visual Perception;Deep Learning in Grasping and Manipulation;Grasping},
  doi={10.1109/LRA.2023.3336108}}
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
            <a class="navbar-item" href="https://twjhlee.github.io/">
              <span class="icon">
                <i class="fas fa-home"></i>
              </span>
            </a>
            <a class="navbar-item" href="https://github.com/twjhlee">
              <span class="icon">
                <i class="fab fa-github"></i>
              </span>
            </a>
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

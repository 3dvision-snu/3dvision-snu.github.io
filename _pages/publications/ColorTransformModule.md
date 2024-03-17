---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/ColorTransformModule
---

<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Robust Novel View Synthesis with Color Transform Module</title>

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
            Robust View Synthesis with Color Transform Module
          </h1>

          <!-- authors -->
          <div class="container is-max-desktop has-text-centered">
            <div class="columns is-mobile is-centered is-gapless">
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://sangminkim-99.github.io/">Sang Min Kim</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://www.changwoon.info/">Changwoon Choi</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="http://3d.snu.ac.kr/members">Hyeongjun Heo</a>
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
            <a class="button link-button is-rounded" href="https://3d.snu.ac.kr/papers/ColorTransformNeRF.pdf">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <a class="button link-button is-rounded" href="https://github.com/sangminkim-99/ColorTransformModule">
              <span class="icon">
                <i class="fab fa-github"></i>
              </span>
              <span>Code</span>
            </a>
            <!-- TODO: add dataset here -->
            <!-- <a
              class="button link-button is-rounded"
              href="https://github.com/82magnolia/n_imagenet?tab=readme-ov-file#downloading-n-imagenet"
            >
              <span class="icon">
                <i class="fa-solid fa-database"></i>
              </span>
              <span>Dataset</span>
            </a> -->
          </div>
        </div>
      </div>
    </section>

    <!-- teasor -->
    <section class="hero">
      <div class="container is-max-desktop">
        <div class="hero-body">
          <img src="{{ site.url }}{{ site.baseurl }}/assets/ColorTransformModule/teaser_modified.jpg" width="100%" style="display: block; margin: auto" />
          <h2 class="subtitle has-text-centered">
            With color transform module, we can accurately reconstruct the geometry and radiance of the low-textured regions.
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
              The advancements of the Neural Radiance Field (NeRF) and its variants have demonstrated remarkable capabilities in generating photo-realistic novel views from a small set of input images. While recent works suggest various techniques and model
              architectures that enhance speed or reconstruction quality, little attention is paid to exploring the RGB color space of input
              images. In this paper, we propose a universal color transform module that can maximally harness the captured evidence for
              the neural networks at hand. The color transform module utilizes an encoder-decoder framework that maps the RGB color
              space into a new latent space, enhancing the expressiveness of the input domain. We attach the encoder and the decoder at the
              input and output of a NeRF model of choice, respectively, and jointly optimize them to maintain the cycle consistency of the
              proposed transform, in addition to minimizing the reconstruction errors in the feature domain. Our comprehensive experiments
              demonstrate that the learned color space can significantly improve the quality of reconstructions compared to the conventional
              RGB representation. Its benefits are particularly pronounced in challenging scenarios characterized by low-light environments
              and scenes with low-textured regions. The proposed color transform pushes the boundaries of limitations in the input domain
              and offers a promising avenue for advancing the reconstruction capabilities of various neural representations.
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
              Method Overview
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/ColorTransformModule/method_overview.jpg" width="100%" style="display: block; margin: auto" />
            <p class="content">
              Our color transform module comprises an encoder <em>f(c)</em> and a decoder <em>g(l)</em>.
    (a) With <em>f(c)</em>, we transform the colors of input images into latent values and train the radiance fields using reconstruction losses in both the transformed and color domains.
    (b) To ensure meaningful values in the latent domain, we incorporate cycle consistency loss as a regularization technique.
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
              Qualitative Results
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/ColorTransformModule/qualitative_result.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              Qualitative results of optimizing NeRF in challenging environments. 
              The first row showcases the rendered images of each scene, with the lower triangle enhanced for better visibility in dark regions. 
              The second row presents the corresponding depth images.
The effectiveness of our CTM is prominent in dark scenes. With a limited color range in
the input image, the vanilla NeRF even does not converge. Our
module not only stabilizes the convergence but also automatically
finds an adequate mapping to increase the performance. We also
noticed that the feature grid of DVGO can sometimes fail to converge despite its fast convergence. 
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
              Comparison Between Other Color Spaces
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/ColorTransformModule/qualitative_colorspace.png"/>
            <p class="content">
              We compare our scene-specific color transformation against existing handcrafted color
              maps. We replace our method with transformations based on HLS, HSV, Lab, and Luv color spaces.
              Additionally, we apply a warping technique to transform the cylindrical positions of the Hue
              channel into Cartesian coordinates (denoted as cart).
              Our method yields the best performance in a challenging scenario.
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
@inproceedings{kim2023robust,
  title={Robust Novel View Synthesis with Color Transform Module},
  author={Kim, SM and Choi, C and Heo, H and Kim, YM},
  booktitle={Computer Graphics Forum},
  volume={42},
  number={7},
  pages={e14931},
  year={2023},
  organization={Wiley Online Library}
}</pre
          >
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
            <a class="navbar-item" href="https://sangminkim-99.github.io/">
              <span class="icon">
                <i class="fas fa-home"></i>
              </span>
            </a>
            <a class="navbar-item" href="https://github.com/sangminkim-99">
              <span class="icon">
                <i class="fab fa-github"></i>
              </span>
            </a>
          </div>
          <!-- <div class="navbar-item has-dropdown has-dropdown-up is-hoverable">
            <a class="navbar-link">More Research</a>

            <div class="navbar-dropdown is-right">
              <a class="navbar-item" href="https://82magnolia.github.io/event_localization/">
                Event-Based Visual Localization
              </a>
              <a class="navbar-item" href="https://github.com/82magnolia/ev_tta">
                Test-Time Adaptation for Event Cameras
              </a>
              <a
                class="navbar-item"
                href="https://openaccess.thecvf.com/content/WACV2023/html/Hwang_Ev-NeRF_Event_Based_Neural_Radiance_Field_WACV_2023_paper.html"
              >
                Event-Based Neural Radiance Fields
              </a>
            </div>
          </div> -->
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

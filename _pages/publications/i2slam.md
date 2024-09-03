---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/i2slam
---

<html data-theme="light">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>I2-SLAM</title>

    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Encode+Sans:wght@300;400;500;600&family=Roboto+Mono&display=swap"
      rel="stylesheet"
    />
    <link href='https://fonts.googleapis.com/css?family=Quicksand' rel='stylesheet'>


    <!-- Bulma -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@1.0.1/css/bulma.min.css" />
    <link rel="stylesheet" href="{{ site.url }}{{ site.baseurl }}/css/project_page_styles/styles_i2slam.css" />
    <script src="{{ site.url }}{{ site.baseurl }}/js/bulma_toggle.js"></script>

    <!-- Font Awesome -->
    <script src="https://kit.fontawesome.com/5fd1dd8417.js" crossorigin="anonymous"></script>

    <!-- Academicons -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css" />
    <link rel="icon" href="{{ site.url }}{{ site.baseurl }}/assets/i2slam/photo-camera-svgrepo-com.svg">

  </head>

  <body>

    <!-- title / authors / icons -->
    <section class="hero">
      <div class="hero-body">
        <div class="container is-max-widescreen has-text-centered">
          <!-- title -->
          <h1 class="title is-size-1 is-size-2-mobile publication-title">
            I<sup>2</sup>-SLAM: Inverting Imaging Process for<br/> Robust Photorealistic Dense SLAM
          </h1>
          <div class="is-size-5-tablet publication-institute">
            <span class="author-block">ECCV 2024</span>
          </div>

          <!-- authors -->
          <div class="container is-max-desktop has-text-centered author-list">
            <div class="columns is-mobile is-centered is-gapless">
              <div class="column is-2-tablet is-size-6-tablet publication-authors">
                <a class="author-blocks" href="https://www.gwangtakbae.info/">Gwangtak Bae<sup><b>*</b></sup></a>
              </div>
              <div class="column is-2-tablet is-size-6-tablet publication-authors">
                <a class="author-blocks" href="https://www.changwoon.info">Changwoon Choi<sup><b>*</b></sup></a>
              </div>
              <div class="column is-2-tablet is-size-6-tablet publication-authors">
                <a class="author-blocks" href="https://3d.snu.ac.kr/members">Hyeongjun Heo</a>
              </div>
              <div class="column is-2-tablet is-size-6-tablet publication-authors">
                <a class="author-blocks" href="https://sangminkim-99.github.io/">Sang Min Kim</a>
              </div>
              <div class="column is-2-tablet is-size-6-tablet publication-authors">
                <a class="author-blocks" href="http://3d.snu.ac.kr/members">Young Min Kim</a>
              </div>
            </div>
          </div>


          <div class="is-size-6-tablet publication-institute">
            <span class="author-block">Seoul National University</span>
            <br/>
            <span class="author-block">(<b>*</b> Equal Contribution)</span>
          </div>

          <!-- logo img -->
          <nav class="navbar logo">
            <div class="navbar-brand logo">
              <a class="navbar-item logo" href="https://3d.snu.ac.kr/">
                <img src="{{ site.url }}{{ site.baseurl }}/images/3dv.png" />
              </a>
            </div>
          </nav>

          <!-- icons -->
          <div class="is-size-5 link-blocks">
            <a class="button link-button is-rounded" href="">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <a class="button link-button is-rounded" href="https://arxiv.org/abs/2407.11347">
              <span class="icon">
                <i class="ai ai-arxiv"></i>
              </span>
              <span>arXiv</span>
            </a>
            <a class="button link-button is-rounded" href="">
              <span class="icon">
                <i class="fa-brands fa-youtube"></i>
              </span>
              <span>Video</span>
            </a>
            <a class="button link-button is-rounded" href="">
              <span class="icon">
                <i class="fab fa-github"></i>
              </span>
              <span>Code</span>
            </a>
          </div>
        </div>
      </div>
    </section>

    <!-- teaser -->
    <section class="hero">
      <div class="container is-max-desktop">
        <div class="hero-body">
          <img class="teaser_video" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/i2slam.gif" style="display: block; margin: auto" />
        </div>
        <h2 class="tldr">
          By inverting imaging process, I<sup>2</sup>-SLAM reconstructs photorealistic and sharp HDR maps <br/>from casually-captured inputs which contain severe motion blur and varying appearances
        </h2>
      </div>
    </section>

    <section class="section">
      <div class="container is-max-desktop">
        <div class="column is-full-width is-centered has-text-centered has-text-left-mobile">
          <h2 class="subtitle is-size-3 has-text-weight-medium publication-keywords">
            Abstract
          </h2>
          <div class="content has-text-justified">
            <p>
              We present an inverse image-formation module that can enhance the robustness of existing visual SLAM pipelines for casually captured scenarios.
              Casual video captures often suffer from motion blur and varying appearances, which degrade the final quality of coherent 3D visual representation.
              We propose integrating the physical imaging into the SLAM system, which employs linear HDR radiance maps to collect measurements.
              Specifically, individual frames aggregate images of multiple poses along the camera trajectory to explain prevalent motion blur in hand-held videos.
              Additionally, we accommodate per-frame appearance variation by dedicating explicit variables for image formation steps, namely white balance, exposure time, and camera response function.
              Through joint optimization of additional variables, the SLAM pipeline produces high-quality images with more accurate trajectories.
              Extensive experiments demonstrate that our approach can be incorporated into recent visual SLAM pipelines using various scene representations, such as neural radiance fields or Gaussian splatting.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="container is-max-desktop">
        <div class="column is-full-width is-centered has-text-centered has-text-left-mobile">
          <h2 class="subtitle is-size-3 has-text-weight-medium publication-keywords">
            Method
          </h2>
          <div class="hero-body">
            <img class="method_overview" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/method_overview.png" style="display: block" />
          </div>
          <div class="content has-text-justified">
            <p>
              We reconstruct a sharp HDR radiance field map.
              Motion blur is simulated by integration of sharp images, which are obtained from virtual camera poses during the exposure time.
              Then we obtain the blurry LDR image by applying differentiable tone mapping module.
              SLAM methods simultaneously perform tracking and mapping from degraded images to reconstruct a sharp HDR map.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="container is-max-desktop">
        <div class="column is-full-width is-centered has-text-centered has-text-left-mobile">
          <h2 class="subtitle is-size-3 has-text-weight-medium publication-keywords">
            Results
          </h2>
          <div class="content has-text-justified">
            <p>
              I<sup>2</sup>-SLAM is a generic module that improves the quality of existing visual SLAM approaches by inverting the image formation process for casually captured videos.
            </p>
          </div>
          <h3 class="column is-size-5 is-full-width has-text-left-mobile has-text-left publication-keywords">
            RGB-D SLAM results in ScanNet dataset
          </h3>
          <div class="fixed-grid has-3-cols">
          <div class="grid">
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/0785_00_00210_input.png" height="100%">
            </div>
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/0785_00_00210_splatam_0.png" height="100%">
            </div>
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/0785_00_00210_ours_2.png" height="100%">
            </div>
            <div class="cell cell_caption" align="center">
              Input frame
            </div>
            <div class="cell cell_caption" align="center">
              SplaTAM
            </div>
            <div class="cell cell_caption" align="center">
              I<sup>2</sup>-SLAM (Ours)
            </div>
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/0736_00_00395_input.png" height="100%">
            </div>
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/0736_00_00395_splatam_1.png" height="100%">
            </div>
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/0736_00_00395_ours_2.png" height="100%">
            </div>
            <div class="cell cell_caption" align="center">
              Input frame
            </div>
            <div class="cell cell_caption" align="center">
              SplaTAM
            </div>
            <div class="cell cell_caption" align="center">
              I<sup>2</sup>-SLAM (Ours)
            </div>
          </div>
          </div>

          <h3 class="column is-size-5 is-full-width has-text-left-mobile has-text-left publication-keywords">
            RGB SLAM results in TUM dataset
          </h3>
          <div class="fixed-grid has-3-cols">
          <div class="grid">
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/fr1_desk_51_input.png" height="100%">
            </div>
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/fr1_desk_51_nerfslam_2.png" height="100%">
            </div>
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/fr1_desk_51_ours_2.png" height="100%">
            </div>
            <div class="cell cell_caption" align="center">
              Input frame
            </div>
            <div class="cell cell_caption" align="center">
              NeRF-SLAM
            </div>
            <div class="cell cell_caption" align="center">
              I<sup>2</sup>-SLAM (Ours)
            </div>
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/fr3_office_135_input.png" height="100%">
            </div>
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/fr3_office_135_nerfslam_0.png" height="100%">
            </div>
            <div class="cell" align="center">
              <img class="results_img" src="{{ site.url }}{{ site.baseurl }}/assets/i2slam/fr3_office_135_ours_0.png" height="100%">
            </div>
            <div class="cell cell_caption" align="center">
              Input frame
            </div>
            <div class="cell cell_caption" align="center">
              NeRF-SLAM
            </div>
            <div class="cell cell_caption" align="center">
              I<sup>2</sup>-SLAM (Ours)
            </div>
          </div>
          </div>
        </div>
      </div>
    </section>

    <!-- BibTex section -->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="column is-full-width is-centered has-text-centered">
          <h2 class="subtitle is-size-3 has-text-weight-medium publication-keywords">BibTeX</h2>
        </div>
        <div class="box bibtex-box">
          <pre>
@InProceedings{I2-SLAM_2024,
  author    = {Bae, Gwangtak and Choi, Changwoon and Heo, Hyeongjun and Kim, Sang Min and Kim, Young Min},
  title     = {I2-SLAM: Inverting Imaging Process for Robust Photorealistic Dense SLAM},
  booktitle = {Proceedings of the European Conference on Computer Vision (ECCV)},
  month     = {},
  year      = {2024},
  pages     = {},
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
            <a class="navbar-item" href="https://changwoon.info">
              <span class="icon">
                <i class="fas fa-home"></i>
              </span>
            </a>
            <a class="navbar-item" href="https://github.com/changwoonchoi">
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

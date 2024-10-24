---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/3Doodle
---

<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>3Doodle</title>

    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Encode+Sans:wght@300;400;500;600&family=Roboto+Mono&display=swap"
      rel="stylesheet"
    />
    <link href='https://fonts.googleapis.com/css?family=Architects Daughter' rel='stylesheet'>
    <link href='https://fonts.googleapis.com/css?family=Quicksand' rel='stylesheet'>


    <!-- Bulma -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@1.0.1/css/bulma.min.css" />
    <link rel="stylesheet" href="{{ site.url }}{{ site.baseurl }}/css/styles.css" />
    <script src="{{ site.url }}{{ site.baseurl }}/js/bulma_toggle.js"></script>

    <!-- Font Awesome -->
    <script src="https://kit.fontawesome.com/5fd1dd8417.js" crossorigin="anonymous"></script>

    <!-- Academicons -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css" />
    <link rel="icon" href="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/favicon.png">
  </head>

  <body>

    <!-- title / authors / icons -->
    <section class="hero">
      <div class="hero-body">
        <div class="container is-max-widescreen has-text-centered">
          <!-- title -->
          <h1 class="title is-size-1 is-size-2-mobile publication-title">
            3Doodle: Compact Abstraction of Objects<br/> with 3D Strokes
          </h1>
          <div class="is-size-5-tablet publication-institute">
            <span class="author-block">SIGGRAPH 2024<br/>(ACM Transactions on Graphics)<br/></span>
          </div>

          <!-- authors -->
          <div class="container is-max-desktop has-text-centered author-list">
            <div class="columns is-mobile is-centered is-gapless">
              <div class="column is-2-tablet is-size-6-tablet publication-authors">
                <a class="author-blocks" href="https://www.changwoon.info">Changwoon Choi<sup>1</sup></a>
              </div>
              <div class="column is-2-tablet is-size-6-tablet publication-authors">
                <a class="author-blocks" href="https://jaeah.me/">Jaeah Lee<sup>2</sup></a>
              </div>
              <div class="column is-2-tablet is-size-6-tablet publication-authors">
                <a class="author-blocks" href="http://jaesik.info">Jaesik Park<sup>2</sup></a>
              </div>
              <div class="column is-2-tablet is-size-6-tablet publication-authors">
                <a class="author-blocks" href="http://3d.snu.ac.kr/members">Young Min Kim<sup>1</sup></a>
              </div>
            </div>
          </div>

          <div class="is-size-6-tablet publication-institute">
            <span class="author-block">Seoul National University</span>
          </div>
          
          <div class="logo-list">
            <a class="lab-logo" href="https://3d.snu.ac.kr">
              <img src="{{ site.url }}{{ site.baseurl }}/images/3dv.png">
            </a>
            <span class="affiliation-num">
              1
            </span>
            <a class="lab-logo" href="https://jaesik.info/lab">
              <img src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/vgilab.png">
            </a>
            <span class="affiliation-num-right">
              2
            </span>
          </div>

          <!-- icons -->
          <div class="is-size-5 link-blocks">
            <a class="button link-button is-rounded" href="./">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <a class="button link-button is-rounded" href="https://arxiv.org/abs/2402.03690">
              <span class="icon">
                <i class="ai ai-arxiv"></i>
              </span>
              <span>arXiv</span>
            </a>
            <a class="button link-button is-rounded" href="https://www.youtube.com/watch?v=7mWPYGRfk-I">
              <span class="icon">
                <i class="fa-brands fa-youtube"></i>
              </span>
              <span>Video</span>
            </a>
            <a class="button link-button is-rounded" href="https://github.com/changwoonchoi/3Doodle">
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
          <img src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/teaser.jpg" width="100%" style="display: block; margin: auto" />
          <h2 class="tldr">
            3Doodle reconstructs <b>3D Strokes</b> from <b>multi-view images</b> without <b>sketch dataset</b>.
          </h2>
        </div>
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
              While free-hand sketching has long served as an efficient representation to convey characteristics of an object, they are often subjective, deviating significantly from realistic representations.
              Moreover, sketches are not consistent for arbitrary viewpoints, making it hard to catch 3D shapes.
              We propose <b>3Doodle</b>, generating descriptive and view-consistent sketch images given multi-view images of the target object.
              Our method is based on the idea that a set of 3D strokes can efficiently represent 3D structural information and render view-consistent 2D sketches.
              We express 2D sketches as a union of view-independent and view-dependent components.
              3D cubic Bézier curves indicate view-independent 3D feature lines, while contours of superquadrics express a smooth outline of the volume of varying viewpoints.
              Our pipeline directly optimizes the parameters of 3D stroke primitives to minimize perceptual losses in a fully differentiable manner.
              The resulting sparse set of 3D strokes can be rendered as abstract sketches containing essential 3D characteristic shapes of various objects.
              We demonstrate that 3Doodle can faithfully express concepts of the original images compared with recent sketch generation approaches
            </p>
          </div>
        </div>
      </div>
    </section>
    <!--
    <section class="section">
      <div class="container is-max-desktop">
        <div class="column is full-width is-centered has-text-centered">
          <h2 class="subtitle is-size-3 has-text-weight-medium publication-keywords">
            Video (todo)
          </h2>
        </div>
        <div class="publication-video">
          <iframe
            src="https://www.youtube.com/embed/7mWPYGRfk-I?si=x0xlB16kK1TOXN_I"
            allow="autoplay; encrypted-media"
            allowfullscreen="true"
          ></iframe>
        </div>
      </div>
    </section>
-->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="column is full-width is-centered has-text-centered">
          <h2 class="subtitle is-size-3 has-text-weight-medium publication-keywords">
            Method
          </h2>
          <img src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/3doodle_method.png" width="90%" style="display: block; margin: auto" />
        </div>
          <p class="normal-text">
            From multiple-view images, we aim to reconstruct view-consistent sketch representation.
            We represent 3D strokes as a union of view-independent and view-dependent components.
            For view-independent components, we use 3D cubic Bézier curves to represent 3D feature lines.
            For view-dependent components, we use contours of superquadrics to express a smooth outline.
            We propose a differentiable rendering pipeline for our 3D stroke representation.
            Then we optimize the compact parameters of 3D stroke primitives to minimize the perceptual loss.
          </p>
      </div>
      </section>

    <section class="section">
      <div class="container is-max-desktop">
        <div class="column is full-width is-centered has-text-centered">
          <h2 class="subtitle is-size-3 has-text-weight-medium publication-keywords">
            Results
          </h2>
        </div>
        <!--NeRF Synthetic results-->
        <div class="fixed-grid has-3-cols">
          <div class="grid">
            <div class="cell" align="center">
              <video class="results_video" id="chair" autoplay controls muted loop playsinline height="100%">
                <source src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/videos/switch_chair.mp4" type="video/mp4">
              </video>
            </div>
          <div class="cell" align="center">
            <video class="results_video" id="ship" autoplay controls muted loop playsinline height="100%">
              <source src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/videos/switch_ship.mp4" type="video/mp4">
            </video>
          </div>
          <div class="cell" align="center">
            <video class="results_video" id="lego" autoplay controls muted loop playsinline height="100%">
              <source src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/videos/switch_lego.mp4" type="video/mp4">
            </video>
          </div>
          <div class="cell" align="center">
            <video class="results_video" id="mic" autoplay controls muted loop playsinline height="100%">
              <source src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/videos/switch_mic.mp4" type="video/mp4">
            </video>
          </div>
          <div class="cell" align="center">
            <video class="results_video" id="hotdog" autoplay controls muted loop playsinline height="100%">
              <source src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/videos/switch_hotdog.mp4" type="video/mp4">
            </video>
          </div>
          <div class="cell" align="center">
            <video class="results_video" id="drums" autoplay controls muted loop playsinline height="100%">
              <source src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/videos/switch_drums.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <p align="center" class="normal-text">
          Results on NeRF synthetic dataset. We use only Bézier curves for this examples.
        </p>
        </div>
        <!--comparison with baselines-->
        <div class="fixed-grid has-1-cols">
          <div class="grid row-gap-0">
            <div class="cell" align="center">
              <video class="comparison_video" autoplay controls muted loop playsinline height="100%">
                <source src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/videos/bigbear_compare.mp4" type="video/mp4">
              </video>
            </div>
            <div class="cell" align="center">
              <video class="comparison_video" autoplay controls muted loop playsinline height="100%">
                <source src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/videos/bigsnow_compare.mp4" type="video/mp4">
              </video>
            </div>
            <div class="cell" align="center">
              <video class="comparison_video" autoplay controls muted loop playsinline height="100%">
                <source src="{{ site.url }}{{ site.baseurl }}/assets/3Doodle/videos/mic_compare.mp4" type="video/mp4">
              </video>
            </div>
          </div>
        </div>
        <div class="fixed-grid has-6-cols caption">
          <div class="grid">
            <div claass="cell" align="center">
              Input
            </div>
            <div claass="cell" align="center">
              NEF
            </div>
            <div claass="cell" align="center">
              ARF
            </div>
            <div claass="cell" align="center">
              Sugg.Contour
            </div>
            <div claass="cell" align="center">
              CLIPasso
            </div>
            <div claass="cell" align="center">
              3Doodle
            </div>
          </div>
        </div>
        <p align="center" class="normal-text">
          Comparison with baselines methods. 
        </p>
        
        
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
          </pre>
          <!--
          <pre>
          @InProceedings{Kim_2021_ICCV,
              author    = {Kim, Junho and Bae, Jaehyeok and Park, Gangin and Zhang, Dongsu and Kim, Young Min},
              title     = {N-ImageNet: Towards Robust, Fine-Grained Object Recognition With Event Cameras},
              booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
              month     = {October},
              year      = {2021},
              pages     = {2146-2156}
          }</pre>
          -->
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
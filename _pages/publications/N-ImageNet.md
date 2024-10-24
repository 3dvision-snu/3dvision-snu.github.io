---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/N-ImageNet
---

<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>N-ImageNet: Towards Robust, Fine-Grained Object Recognition with Event Cameras</title>

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
            N-ImageNet: Towards Robust, Fine-Grained <br />Object Recognition with Event Cameras
          </h1>

          <!-- authors -->
          <div class="container is-max-desktop has-text-centered">
            <div class="columns is-mobile is-centered is-gapless">
              <div class="column is-2-tablet is-size-5 publication-authors">
                <a class="author-blocks" href="https://www.junhokim.xyz">Junho Kim</a>
              </div>
              <div class="column is-2-tablet is-size-5 publication-authors">
                <a class="author-blocks" href="http://3d.snu.ac.kr/members">Jaehyeok Bae</a>
              </div>
              <div class="column is-2-tablet is-size-5 publication-authors">
                <a class="author-blocks" href="http://3d.snu.ac.kr/members">Gangin Park</a>
              </div>
              <div class="column is-2-tablet is-size-5 publication-authors">
                <a class="author-blocks" href="http://dszhang.me/about">Dongsu Zhang</a>
              </div>
              <div class="column is-2-tablet is-size-5 publication-authors">
                <a class="author-blocks" href="http://3d.snu.ac.kr/members">Young Min Kim</a>
              </div>
            </div>
          </div>

          <div class="is-size-5 publication-institute">
            <span class="author-block">Dept. of Electrical and Computer Engineering, Seoul National University</span>
          </div>

          <!-- icons -->
          <div class="is-size-5 link-blocks">
            <a class="button link-button is-rounded" href="{{ site.url }}{{ site.baseurl }}/assets/N-ImageNet/paper.pdf">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <a class="button link-button is-rounded" href="https://arxiv.org/abs/2112.01041">
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
            <a class="button link-button is-rounded" href="https://github.com/82magnolia/n_imagenet">
              <span class="icon">
                <i class="fab fa-github"></i>
              </span>
              <span>Code</span>
            </a>
            <a
              class="button link-button is-rounded"
              href="https://github.com/82magnolia/n_imagenet?tab=readme-ov-file#downloading-n-imagenet"
            >
              <span class="icon">
                <i class="fa-solid fa-database"></i>
              </span>
              <span>Dataset</span>
            </a>
          </div>
        </div>
      </div>
    </section>

    <!-- teasor -->
    <section class="hero">
      <div class="container is-max-desktop">
        <div class="hero-body">
          <img src="{{ site.url }}{{ site.baseurl }}/assets/N-ImageNet/qualitative.png" width="75%" style="display: block; margin: auto" />
          <h2 class="subtitle has-text-centered">
            N-ImageNet is a large-scale, fine-grained dataset for event-based object recognition.
          </h2>
        </div>
      </div>
    </section>

    <!-- content section with left-side subtitle -->
    <section class="section">
      <div class="container is-max-desktop">
        <!-- abstract -->
        <div class="columns">
          <div class="column is-one-fifth has-text-centered">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Abstract</h2>
          </div>
          <div class="column has-text-justified">
            <p class="content">
              We introduce N-ImageNet, a large-scale dataset targeted for robust, fine-grained object recognition with
              event cameras. The dataset is collected using programmable hardware in which an event camera consistently
              moves around a monitor displaying images from ImageNet. N-ImageNet serves as a challenging benchmark for
              event-based object recognition, due to its large number of classes and samples. We empirically show that
              pretraining on N-ImageNet improves the performance of event-based classifiers and helps them learn with
              few labeled data. In addition, we present several variants of N-ImageNet to test the robustness of
              event-based classifiers under diverse camera trajectories and severe lighting conditions, and propose a
              novel event representation to alleviate the performance degradation. To the best of our knowledge, we are
              the first to quantitatively investigate the consequences caused by various environmental conditions on
              event-based object recognition algorithms. N-ImageNet and its variants are expected to guide practical
              implementations for deploying event-based object recognition algorithms in the real world.
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
                src="https://www.youtube.com/embed/7mWPYGRfk-I?si=x0xlB16kK1TOXN_I"
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
              What Are Event Cameras?
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/N-ImageNet/events.gif" width="90%" style="display: block; margin: auto" />
            <p class="content">
              Event cameras are neuromorphic sensors that encode visual information as a sequence of events. In contrast
              to conventional frame-based cameras that output absolute brightness intensities, event cameras respond to
              brightness changes. The following figure shows a visual description of how event cameras function compared
              to conventional cameras. Notice how brightness changes are encoded as 'streams' in the spatio-temporal
              domain.
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
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Dataset Overview</h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/N-ImageNet/dataset_overview.png" width="85%" style="display: block; margin: auto" />
            <p class="content">
              N-ImageNet is a large-scale event dataset that enables training and benchmarking object recongition
              algorithms using event camera input. The dataset surpasses all existing datasets in both size and label
              granularity.
            </p>
          </div>
        </div>

        <div class="columns">
          <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">
              Data Acquisition Setup
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/N-ImageNet/hardware.png" width="85%" style="display: block; margin: auto" />
            <p class="content">
              To capture N-ImageNet, we design custom hardware to trigger perpetual camera motion. The device consists
              of two geared motors connected to a pair of perpendicularly adjacent gear racks where the upper and lower
              motors are responsible for vertical and horizontal motion, respectively. Each motor is further linked to a
              programmable Arduino board, which can control the camera movement.
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
              Object Recognition Performance Analysis
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/N-ImageNet/performance.png" width="80%" style="display: block; margin: auto" />
            <p class="content">
              Due to its size and label diversity, N-ImageNet can function as a challenging benchmark for event-based
              object recognition. The plot below shows the classification accuracy of existing event-based recognition
              algorithms on N-ImageNet. There exists a large performance gap with the ImageNet state-of-the-art, which
              suggests that mastering N-ImageNet is still a long way to go. We expect N-ImageNet to foster development
              of event classifiers that could readily function in the real world.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Content section with centered subtitle -->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="column is-full-width is-centered has-text-centered has-text-left-mobile">
          <h2 class="subtitle is-size-3 has-text-weight-medium publication-keywords">
            Useful Links for Benchmarking and Downloading
          </h2>
          <div class="content has-text-justified">
            <p>
              <b>Public Benchmark: </b> Check out the public benchmark on event-based object recognition available at
              the following <a href="https://paperswithcode.com/dataset/n-imagenet">link</a>. Feel free to upload new
              results to the benchmark!
            </p>
            <p>
              <b>Downloading Full N-ImageNet: </b> Refer to the following
              <a
                href="https://docs.google.com/document/d/1x0Vqe_5tVAJtYLYSZLwN6oNMExyUjIh-a30oLOKV2rE/edit?usp=share_link"
                >link</a
              >
              to download N-ImageNet. Note the full dataset size will be around 400 GB, so prepare a sufficient amount
              of disk space before downloading! Please leave an email to
              <a href="mailto:82magnolia@snu.ac.kr">Junho Kim</a> if you are in urgent need of N-ImageNet and the file
              share links are not working.
            </p>
            <p>
              <b
                >Downloading Mini
                <span class="icon-text">
                  <span class="icon">
                    <i class="fa-solid fa-baby"></i>
                  </span>
                  <span>N-ImageNet:</span>
                </span>
              </b>
              Starting from 2022, we publicly released a smaller version of N-ImageNet, called mini N-ImageNet. The
              dataset contains 100 classes, which is 1/10 of the original N-ImageNet. We expect the dataset to enable
              quick and light-weight evaluation of new event-based object recognition methods. To download the dataset,
              please refer to the follwoing
              <a href="https://zenodo.org/record/6388221#.Y51iJNJBw5k">link</a>.
            </p>
            <p>
              <b>Downloading Pretrained Models: </b> To download the pretrained models, refer to the following
              <a href="https://github.com/82magnolia/n_imagenet?tab=readme-ov-file#downloading-pretrained-models"
                >link</a
              >.
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
@InProceedings{Kim_2021_ICCV,
    author    = {Kim, Junho and Bae, Jaehyeok and Park, Gangin and Zhang, Dongsu and Kim, Young Min},
    title     = {N-ImageNet: Towards Robust, Fine-Grained Object Recognition With Event Cameras},
    booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
    month     = {October},
    year      = {2021},
    pages     = {2146-2156}
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
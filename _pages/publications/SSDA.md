---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/SSDA
---

<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Self-Supervised Domain Adaptation for Visual Navigation with Global Map Consistency</title>

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
            Self-Supervised Domain Adaptation for <br />Visual Navigation with Global Map Consistency
          </h1>

          <!-- authors -->
          <div class="container is-max-desktop has-text-centered">
            <div class="columns is-mobile is-centered is-gapless">
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://eunsunlee.github.io">Eun Sun Lee</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://www.junhokim.xyz">Junho Kim</a>
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
            <a class="button link-button is-rounded" href="{{ site.url }}{{ site.baseurl }}/assets/SSDA/paper.pdf">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <a class="button link-button is-rounded" href="https://arxiv.org/abs/2110.07184">
              <span class="icon">
                <i class="ai ai-arxiv"></i>
              </span>
              <span>arXiv</span>
            </a>
            <a class="button link-button is-rounded" href="https://www.youtube.com/watch?v=7nqUENuDp9E">
              <span class="icon">
                <i class="fa-brands fa-youtube"></i>
              </span>
              <span>Video</span>
            </a>
          </div>
        </div>
      </div>
    </section>

    <!-- teasor -->
    <section class="hero">
      <div class="container is-max-desktop">
        <div class="hero-body">
          <img src="{{ site.url }}{{ site.baseurl }}/assets/SSDA/fig1.png" width="90%" style="display: block; margin: auto" />
          <h2 class="subtitle has-text-centered">
            Our study suggests a self-supervised domain adaptation method which generalize a pretrained visual navigation agent to unseen environment with global map consistency.
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
              We propose a light-weight, self-supervised adaptation for a visual navigation agent to generalize to unseen environment. 
              Given an embodied agent trained in a noiseless environment, our objective is to transfer the agent to a noisy environment 
              where actuation and odometry sensor noise is present. Our method encourages the agent to maximize the consistency between 
              the global maps generated at different time steps in a round-trip trajectory. The proposed task is completely self-supervised, 
              not requiring any supervision from ground-truth pose data or explicit noise model. In addition, optimization of the task 
              objective is extremely light-weight, as training terminates within a few minutes on a commodity GPU. Our experiments show that
              the proposed task helps the agent to successfully transfer to new, noisy environments. The transferred agent exhibits improved 
              localization and mapping accuracy, further leading to enhanced performance in downstream visual navigation tasks. Moreover, 
              we demonstrate test-time adaptation with our self-supervised task to show its potential applicability in real-world deployment.
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
                src="https://www.youtube.com/embed/7nqUENuDp9E?si=x0xlB16kK1TOXN_I"
                allow="autoplay; encrypted-media"
                allowfullscreen="true"
              ></iframe>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- content section with left-side subtitle -->
    <!-- <section class="section">
      <div class="container is-max-desktop">
        <div class="columns">
          <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">
              Demo Video
            </h2>
          </div>
          <div class="column has-text-justified">
            <video controls="controls" width="800" height="600" name="Video Name">
              <source src="{{ site.url }}{{ site.baseurl }}/assets/SSDA/MoDA.mov">
            </video>
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
    </section> -->

    <!-- Content section with left-side subtitle -->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="columns">
          <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Global Map Consistency from a Round Trip</h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/SSDA/fig2.png" width="80%" style="display: block; margin: auto" />
            <p class="content">
              We can create a supervision signal by enforcing consistency of the generated global map. While we cannot assure that
              the map is error-free, we can assume that the error accumulates over time. This leads to incorporating more accurate
              pose data in generating the global map in the earlier steps compared to the ones generated later in a continuing trajectory.
              To implement the self-supervised learning task efficiently, we deliberately design overlapping trajectories and
              drive an embodied agent in round trips. The global map is first generated during the forward path, then the agent 
              resets and generates another map from scratch during the backward path. In a noiseless setting, the agent observes 
              the same area at each one-way trip. Therefore, the global map from its forward path should be equal to the global 
              map generated during its backward path. When the actuation noise is present, the agent may not step on the same 
              waypoints it has traversed during its forward path. Nonetheless, our proposed formulation is still valid as the 
              agent generates maps from the overlapping area.
            </p>
          </div>
        </div>

        <div class="columns">
          <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">
              Data Augmentation
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/SSDA/fig3.png" width="85%" style="display: block; margin: auto" />
            <p class="content">
              While our vanilla formulation utilize the bisections of round-trip trajectories, the consistency
              can be enforced for any subsets of trajectories with overlapping observations. We introduce a data augmentation
              method based on random cropping which has been used in various types of data such as videos or images. 
              As shown in the image above, a round trip trajectory can be augmented by randomly sampling the three time steps, initial time, t1,
              the turn time, to, and the end time, t2, in a chronological order.
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
              Experiment Result
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/SSDA/fig4.png" width="85%" style="display: block; margin: auto" />
            <p class="content">
              We extensively evaluate the performance of a pre-trained embodied agent when adapted to a new environment with
              our self-supervised learning task. We first investigate if our proposed self-supervised learning task helps agents
              to transfer to a new, noisy environment. We pre-train an agent in a noiseless environment
              where the mapping and localization module is trained with the ground-truth pose and egocentric map. We then
              observe if our self-supervision can help the agent to generalize across various unseen noisy environments without
              ground-truth supervision. For unseen noisy environment, we apply the odometry noise and actuation noise models
              based on real data of LoCoBot. For each episode, we report the localization error and the
              mean squared error (MSE) of the generated occupancy grid maps with respect to the ground-truth maps. In our paper,
              we show our result for exploration since it is the fundamental task for most navigation agents.

            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Content section with centered subtitle
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
    </section> -->

    <!-- BibTex sectoion -->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="column is-full-width is-centered has-text-centered">
          <h2 class="subtitle is-size-3 has-text-weight-medium publication-keywords">BibTeX</h2>
        </div>
        <div class="box bibtex-box">
          <pre>
@inproceedings{lee2022self,
  title={Self-supervised domain adaptation for visual navigation with global map consistency},
  author={Lee, Eun Sun and Kim, Junho and Kim, Young Min},
  booktitle={Proceedings of the IEEE/CVF winter conference on applications of computer vision},
  pages={1707--1716},
  year={2022}
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
            <a class="navbar-item" href="https://sites.google.com/view/eunsunlee">
              <span class="icon">
                <i class="fas fa-home"></i>
              </span>
            </a>
            <a class="navbar-item" href="https://github.com/eunsunlee">
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

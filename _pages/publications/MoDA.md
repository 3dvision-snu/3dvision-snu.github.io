---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/MoDA
---

<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>MoDA: Map style transfer for self-supervised Domain Adaptation of embodied agents</title>

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
            MoDA: Map style transfer for self-supervised<br />Domain Adaptation of embodied agents
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
            <a class="button link-button is-rounded" href="{{ site.url }}{{ site.baseurl }}/assets/MoDA/paper.pdf">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <a class="button link-button is-rounded" href="https://arxiv.org/abs/2211.15992">
              <span class="icon">
                <i class="ai ai-arxiv"></i>
              </span>
              <span>arXiv</span>
            </a>
            <a class="button link-button is-rounded" href="https://www.youtube.com/watch?v=j7u47WUZESI">
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
          <img src="{{ site.url }}{{ site.baseurl }}/assets/MoDA/fig1.png" width="90%" style="display: block; margin: auto" />
          <h2 class="subtitle has-text-centered">
            MoDA is a domain adaptation method which transfers a pretrained embodied agent to a new, noisy environment without ground-truth supervision.
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
              We propose a domain adaptation method, MoDA, which adapts a pretrained embodied agent to a new, noisy 
              environment without ground-truth supervision. Map-based memory provides important contextual information
              for visual navigation, and exhibits unique spatial structure mainly composed of flat walls and rectangular 
              obstacles. Our adaptation approach encourages the inherent regularities on the estimated maps to guide 
              the agent to overcome the prevalent domain discrepancy in a novel environment. Specifically, we propose 
              an efficient learning curriculum to handle the visual and dynamics corruptions in an online manner, 
              self-supervised with pseudo clean maps generated by style transfer networks. Because the map-based 
              representation provides spatial knowledge for the agent’s policy, our formulation can deploy the pretrained 
              policy networks from simulators in a new setting. We evaluate MoDA in various practical scenarios and show 
              that our proposed method quickly enhances the agent’s performance in downstream tasks including localization, 
              mapping, exploration, and point-goal navigation.
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
                src="https://www.youtube.com/embed/j7u47WUZESI?si=x0xlB16kK1TOXN_I"
                allow="autoplay; encrypted-media"
                allowfullscreen="true"
              ></iframe>
            </div>
          </div>
        </div>
      </div>
    </section>


    <!-- Content section with left-side subtitle -->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="columns">
          <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Unpaired map-to-map translation network</h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/MoDA/fig3.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              MoDA suggests an integrated domain adaptation method for visual and dynamics corruptions,
               which fine-tunes an agent in an efficient learning curriculum. The agent collects a new map dataset 
               to learn map style transfer networks. 
               Given the set of ground-truth maps D<sub>gt</sub>(grey) obtained from the noiseless simulator, 
               the set of noisy maps D<sub>noisy</sub>(green) is collected by the pretrained agent deployed in a novel environment 
               amidst visual and dynamics corruptions.
              We then learn two map-to-map translation networks for the egocentric map S<sup>ego</sup>(yellow) and global map S<sup>global</sup> (blue)
               to translate the maps in D<sub>noisy</sub>into the style of the maps in D<sub>gt</sub>.
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
              Demo Video
            </h2>
          </div>
          <div class="column has-text-justified">
            <video controls="controls" width="800" height="600" name="Video Name">
              <source src="{{ site.url }}{{ site.baseurl }}/assets/MoDA/MoDA.mov">
            </video>
            <p class="content">
              This video shows a demo of a navigation agent's exploration performance under visual and dynamics corruptions with and without adaptation. 
              We use the Habitat simulator and unseen scenes of Gibson and Matterport3D for evaluation. 
            
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
            <img src="{{ site.url }}{{ site.baseurl }}/assets/MoDA/fig5.png" width="85%" style="display: block; margin: auto" />
            <p class="content">
              Qualitative result of mapping (top) and localization (bottom) obtained from agents observing the 
              identical sequence of RGB observations and odometry sensor readings. 
              The reconstructed maps (blue) are aligned on the ground-truth maps (grey), 
              and the estimated pose trajectories (blue line) are compared to the ground-truth trajectories (red line).
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
@inproceedings{lee2022moda,
  title={MoDA: Map style transfer for self-supervised Domain Adaptation of embodied agents},
  author={Lee, Eun Sun and Kim, Junho and Park, SangWon and Kim, Young Min},
  booktitle={European Conference on Computer Vision},
  pages={338--354},
  year={2022},
  organization={Springer}
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

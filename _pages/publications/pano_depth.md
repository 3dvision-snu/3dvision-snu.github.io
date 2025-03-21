---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/pano_depth
---

<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Calibrating Panoramic Depth Estimation for Practical Localization and Mapping</title>

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
            Calibrating Panoramic Depth Estimation for Practical Localization and Mapping
          </h1>

          <!-- authors -->
          <div class="container is-max-desktop has-text-centered">
            <div class="columns is-mobile is-centered is-gapless">
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://www.junhokim.xyz">Junho Kim</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://sites.google.com/view/eunsunlee">Eunsun Lee</a>
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
            <a class="button link-button is-rounded" href="{{ site.url }}{{ site.baseurl }}/assets/pano_depth/paper.pdf">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <a class="button link-button is-rounded" href="https://arxiv.org/abs/2308.14005">
              <span class="icon">
                <i class="ai ai-arxiv"></i>
              </span>
              <span>arXiv</span>
            </a>
            <a class="button link-button is-rounded" href="https://www.youtube.com/watch?v=KXz8IwrtJWg">
              <span class="icon">
                <i class="fa-brands fa-youtube"></i>
              </span>
              <span>Video</span>
            </a>
            <a class="button link-button is-rounded" href="https://github.com/82magnolia/panoramic-depth-calibration">
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
          <img src="{{ site.url }}{{ site.baseurl }}/assets/pano_depth/overview.png" width="85%" style="display: block; margin: auto" />
          <h2 class="subtitle has-text-centered">
            We propose a <b>calibration scheme</b> that adapts a pre-trained panoramic depth estimation network to new, unseen environments using light-weight training objectives.
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
              The absolute depth values of surrounding environments
              provide crucial cues for various assistive technologies, such
              as localization, navigation, and 3D structure estimation.
              We propose that accurate depth estimated from panoramic
              images can serve as a powerful and light-weight input for a
              wide range of downstream tasks requiring 3D information.
              While panoramic images can easily capture the surrounding context from commodity devices, the estimated depth
              shares the limitations of conventional image-based depth
              estimation; the performance deteriorates under large domain shifts and the absolute values are still ambiguous to
              infer from 2D observations. By taking advantage of the
              holistic view, we mitigate such effects in a self-supervised
              way and fine-tune the network with geometric consistency
              during the test phase. Specifically, we construct a 3D
              point cloud from the current depth prediction and project
              the point cloud at various viewpoints or apply stretches on
              the current input image to generate synthetic panoramas.
              Then we minimize the discrepancy of the 3D structure estimated from synthetic images without collecting additional
              data. We empirically evaluate our method in robot navigation and map-free localization where our method shows
              large performance enhancements. Our calibration method
              can therefore widen the applicability under various external conditions, serving as a key component for practical
              panorama-based machine vision systems.
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
                src="https://www.youtube.com/embed/KXz8IwrtJWg?si=Um-XmVtWWjdMmYNT"
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
              Why Panoramic Depth Estimation?
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/pano_depth/why_pano.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              Given a single panorama image, panoramic depth estimation outputs a dense depth map from pre-trained neural networks.
              Since a full-surround 3D map is obtainable from a single neural network inference, panoramic depth estimation can enable light-weight 3D map creation.              
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
              Challenges in Panoramic Depth Estimation
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/pano_depth/pano_challenge.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              One of the key challenges in panoramic depth estimation is the <b>small size of depth-annotated panoramic datasets</b> compared to the regular field-of-view counterparts.
              As a result, existing panoramic depth estimation methods fail to generalize in domain shifts that occur during deployment.              
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
              Panoramic Depth Calibration Overview
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/pano_depth/calibration_overview.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              Given a network pre-trained on large number of panorama images, our calibration scheme aims to enhance its performance in new, unseen environments by training the network on a small number of test samples.              
              Note the training does not leverage any ground-truth annotations.
              The calibrated network can produce more accurate 3D maps, which will be beneficial for downstream applications such as navigation.
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
              Training Objectives (Normal and Chamfer Loss)
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/pano_depth/multi_view_loss.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              Our calibration scheme utilizes three loss functions.
              The <b>multi-view loss functions (normal & chamfer)</b> operate by synthesizing panoramas at random pose perturbations.
              Given the synthesized panoramas and their depth predictions,
              chamfer loss enforces the point cloud coordinates produced from the two depth maps to be similar,
              and normal loss additionally enforces the point cloud normals to be similar.              
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
              Training Objectives (Stretch Loss)
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/pano_depth/stetch_loss.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              <b>Stretch loss</b> further imposes depth map consistency against stretched panoramas.
              The loss specifically targets small or large-scale scenes, where we empirically observed depth estimation errors to largely increase compared to other sources of domain shifts.
              To elaborate, we synthesize panoramas at various stretch rates, and impose depth map consistencies against each stretched panorama.              
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
              Evaluation Setup
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/pano_depth/eval_setup.png" width="80%" style="display: block; margin: auto" />
            <p class="content">
              We test our calibration method on a wide variety of domain shifts that could occur in robotics or AR/VR applications.
              Specifically, we consider global lighting changes (image gamma, white balance, low lighting), image noises (gaussian, speckle, salt and pepper), and geometric changes (scene scale change to large/small scenes, camera rotation).
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
              Quantitative Results
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/pano_depth/quantitative.png" width="80%" style="display: block; margin: auto" />
            <p class="content">
              The plot shown here delineates the mean absolute error (MAE) of various adaptation methods tested in the Stanford2D-3D-S and OmniScenes datasets.
              Our method outperforms the baselines under the aforementioned domain shifts, with more than 10cm decrease in MAE in most cases.
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
              Qualitative Results
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/pano_depth/qualitative.png" width="90%" style="display: block; margin: auto" />
            <p class="content">
              Here we show qualitative results of depth estimation before and after applying our calibration scheme.
              Prior to calibration, depth maps are very noisy due to the salt and peppr noise shown on the left.
              By applying our calibration scheme, the depth maps better align with the ground-truth shown in green.

              <img src="{{ site.url }}{{ site.baseurl }}/assets/pano_depth/ThumbnailAnimatedv4.gif" width="90%" style="display: block; margin: auto" />

              Here's an animation showing the depth estimation results obtained from our calibration scheme.
              While the initial depth estimation network produces noisy depth estimates, the calibration leads to enhanced depth predictions after a few training iterations.
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
@InProceedings{Kim_2023_ICCV,
  author    = {Kim, Junho and Lee, Eun Sun and Kim, Young Min},
  title     = {Calibrating Panoramic Depth Estimation for Practical Localization and Mapping},
  booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
  month     = {October},
  year      = {2023},
  pages     = {8830-8840}
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
              <a class="navbar-item" href="https://github.com/82magnolia/panoramic-localization">
                Panoramic Localization
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

---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/EvTTA
---

<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Ev-TTA: Test-Time Adaptation for Event-Based Object Recognition</title>

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
            Ev-TTA: Test-Time Adaptation <br>for Event-Based Object Recognition
          </h1>

          <!-- authors -->
          <div class="container is-max-desktop has-text-centered">
            <div class="columns is-mobile is-centered is-gapless">
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://www.junhokim.xyz">Junho Kim</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://inwoohwang.me">Inwoo Hwang</a>
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
            <a class="button link-button is-rounded" href="{{ site.url }}{{ site.baseurl }}/assets/EvTTA/paper.pdf">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <a class="button link-button is-rounded" href="https://arxiv.org/abs/2203.12247">
              <span class="icon">
                <i class="ai ai-arxiv"></i>
              </span>
              <span>arXiv</span>
            </a>
            <a class="button link-button is-rounded" href="https://www.youtube.com/watch?v=H4D7gDHn7oI">
              <span class="icon">
                <i class="fa-brands fa-youtube"></i>
              </span>
              <span>Video</span>
            </a>
            <a class="button link-button is-rounded" href="https://github.com/82magnolia/ev_tta">
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
          <img src="{{ site.url }}{{ site.baseurl }}/assets/EvTTA/overview.png" width="90%" style="display: block; margin: auto" />
          <h2 class="subtitle has-text-centered">
            Ev-TTA is a simple, effective <b>test-time adaptation method</b> for event-based object recognition.
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
              We introduce Ev-TTA, a simple, effective test-time adaptation algorithm for event-based object recognition. While
              event cameras are proposed to provide measurements of
              scenes with fast motions or drastic illumination changes,
              many existing event-based recognition algorithms suffer
              from performance deterioration under extreme conditions
              due to significant domain shifts. Ev-TTA mitigates the
              severe domain gaps by fine-tuning the pre-trained classifiers during the test phase using loss functions inspired
              by the spatio-temporal characteristics of events. Since the
              event data is a temporal stream of measurements, our loss
              function enforces similar predictions for adjacent events to
              quickly adapt to the changed environment online. Also,
              we utilize the spatial correlations between two polarities of
              events to handle noise under extreme illumination, where
              different polarities of events exhibit distinctive noise distributions. Ev-TTA demonstrates a large amount of performance gain on a wide range of event-based object recognition tasks without extensive additional training. Our formulation can be successfully applied regardless of input representations and further extended into regression tasks. We
              expect Ev-TTA to provide the key technique to deploy eventbased vision algorithms in challenging real-world applications where significant domain shift is inevitable.
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
                src="https://www.youtube.com/embed/H4D7gDHn7oI?si=fUusZaCw8NDqlCUn"
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
            <img src="{{ site.url }}{{ site.baseurl }}/assets/EvTTA/events.gif" width="90%" style="display: block; margin: auto" />
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
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Problem Setup (Sensing-Perception Gap)</h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/EvTTA/sensing_perception_gap.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              Event cameras can provide measurements in extreme conditions due to the hardware-level benefits such as high dynamic range and temporal resolution.
              However, the classifiers trained on event captures from normal conditions do not generalize well in such challenging scenarios.
              Thus a <b>sensing-perception gap</b> exists, where the visual sensor can provide robust measurements while the entailing perception algorithms cannot properly handle the domain gaps.
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
              Method Overview
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/EvTTA/method.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              Ev-TTA mitigates the domain gaps from extreme measurement conditions by fine-tuning the classifier during test phase.
              Consider a model trained with ground truth labels on the source domain as seen on the left which will make low quality predictions in novel, unseen environments.
              Ev-TTA adapts this model to new conditions <b>without using ground truth labels in an online manner</b>.
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
              Training Objectives (Prediction Similarity Loss)
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/EvTTA/prediction_simlarity.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              Ev-TTA exploits two loss functions for adaptation.
              <b>Prediction similarity loss</b> enforces the predictions made on various regions in the event stream to follow the prediction on the anchor event which is shown as the red box.
              The loss is a symmetric KL divergence which penalizes deviations between the anchor event prediction and the rest.
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
              Training Objectives (Selective Entropy Loss)
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/EvTTA/selective_entropy.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              <b>Selective entropy loss</b> enhances the quality of the anchor prediction.
              The loss minimizes the prediction entropy of the anchor event if its prediction is consistent with predictions made on the neighboring events.
              Here the consistency is determined by comparing the class prediction of the anchor event against the majority vote made from the neighboring events.
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
              Denoising for Low Light Conditions
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/EvTTA/denoising.png" width="70%" style="display: block; margin: auto" />
            <p class="content">
              In low light conditions, Ev-TTA additionally performs denoising using spatial consistency.
              Large amounts of noise on a single event polarity often occur in low light conditions, which can be observed on the negative polarity in the figure.
              For each event on the polarity where noise occurred, we examine its neighbors in the opposite polarity and if the event lacks any neighbors, we label it as noise and remove it.
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
              Adaptation Performance Analysis
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/EvTTA/qual_results.png" width="80%" style="display: block; margin: auto" />
            <p class="content">
              The curves above show the classification accuracy of Ev-TTA measured in N-ImageNet, a large-scale benchmark for event-based object recognition.
              The dataset contains evaluation splits with events obtained under <b>brightness changes</b> (e.g., low light) and <b>camera trajectory changes</b> (e.g., fast motion).
              Compared to <i>no adaptation</i>, large amounts of accuracy improvements exist, and the accuracy approaches results from <i>ground-truth training</i> when given more test-time training data.
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
@InProceedings{Kim_2022_CVPR,
  author    = {Kim, Junho and Hwang, Inwoo and Kim, Young Min},
  title     = {Ev-TTA: Test-Time Adaptation for Event-Based Object Recognition},
  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
  month     = {June},
  year      = {2022},
  pages     = {17745-17754}
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

---
title: "3D Vision Lab"
layout: projects
excerpt: "3D Vision Lab at Seoul National University."
sitemap: false
permalink: /publications/DynamicMeshRecovery
---

<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Dynamic Mesh Recovery from Partial Point Cloud Sequence</title>

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
            Dynamic Mesh Recovery from Partial Point Cloud Sequence
          </h1>

          <!-- authors -->
          <div class="container is-max-desktop has-text-centered">
            <div class="columns is-mobile is-centered is-gapless">
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://hojunjang17.github.io/">Hojun Jang</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="http://3d.snu.ac.kr/members">Minkwan Kim</a>
              </div>
              <div class="column is-2-tablet is-size-5-tablet publication-authors">
                <a class="author-blocks" href="https://jinseokbae.github.io/">Jinseok Bae</a>
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
            <a class="button link-button is-rounded" href="https://openaccess.thecvf.com/content/ICCV2023/html/Jang_Dynamic_Mesh_Recovery_from_Partial_Point_Cloud_Sequence_ICCV_2023_paper.html">
              <span class="icon">
                <i class="fa-solid fa-file"></i>
              </span>
              <span>Paper</span>
            </a>
            <!--
            <a class="button link-button is-rounded" href="https://arxiv.org/abs/2112.01041">
              <span class="icon">
                <i class="ai ai-arxiv"></i>
              </span>
              <span>arXiv</span>
            </a>
          -->
            <a class="button link-button is-rounded" href="https://youtu.be/OgineYrkgRE">
              <span class="icon">
                <i class="fa-brands fa-youtube"></i>
              </span>
              <span>Video</span>
            </a>
            <a class="button link-button is-rounded" href="https://github.com/hojunJang17/DynamicMeshRecovery">
              <span class="icon">
                <i class="fab fa-github"></i>
              </span>
              <span>Code</span>
            </a>
            <!--
            <a
              class="button link-button is-rounded"
              href="https://github.com/82magnolia/n_imagenet?tab=readme-ov-file#downloading-n-imagenet"
            >
              <span class="icon">
                <i class="fa-solid fa-database"></i>
              </span>
              <span>Dataset</span>
            </a>
          -->
          </div>
        </div>
      </div>
    </section>

    <!-- teasor -->
    <section class="hero">
      <div class="container is-max-desktop">
        <div class="hero-body">
          <img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/teaser.png" width="70%" style="display: block; margin: auto" />
          <h2 class="subtitle has-text-centered">
            Reusable 3D kinematic priors from large-scale motion dataset can provide strong structural semantics to recover dynamic 3D mesh in various scenarios.
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
              The exact 3D dynamics of the human body provides crucial evidence to analyze the consequences of the physical interaction between the body and the environment, which can eventually assist everyday activities in a wide range of applications. However, optimizing for 3D configurations from image observation requires a significant amount of computation, whereas real-world 3D measurements often suffer from noisy observation or complex occlusion. We resolve the challenge by learning a latent distribution representing strong temporal priors. We use a conditional variational autoencoder (CVAE) architecture with a transformer to train the motion priors with a large-scale motion dataset. Then our feature follower effectively aligns the feature spaces of noisy, partial observation with the necessary input for pre-trained motion priors, and quickly recovers a complete mesh sequence of motion. We demonstrate that the transformer-based autoencoder can collect necessary spatio-temporal correlations robust to various adversaries, such as missing temporal frames, or noisy observation under severe occlusion. Our framework is general and can be applied to recover the full 3D dynamics of other subjects with parametric representations.
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
                src="https://youtube.com/embed/OgineYrkgRE?si=cVGovUe9QA0vrOfL"
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
              Method Overview
            </h2>
          </div>
          <div class="column has-text-justified">
            <img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/method_new.png" width="100%" style="display: block; margin: auto" />
            <p class="content">
              The <b><font color='gray'>Kinematics Learner</font></b>, the point cloud feature encoder followed by the parameter estimator, learns how to recover mesh from the complete point cloud sequence input.
              The <b><font color='#1e81b0'>Feature Follower</font></b> then follows the encoding of the feature encoder in the kinematics learner.
              The learning of the feature encoding makes our model to effectively handle noisy, partial point cloud sequence inputs.
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
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Qualitative Results<br><font size="3em">(Human, Synthetic)</font></h2>
          </div>
          <div class="column has-text-justified">
            <table>
              <tr>
                <th style="text-align:center">Input</th>
                <th style="text-align:center">Ours</th>
                <th style="text-align:center">VoteHMR</th>
                <th style="text-align:center">Zuo <i>et al.</i></th>
              </tr>
              <tr>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_input_10.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_ours_10.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_votehmr_10.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_zuo_10.gif"/></td>
              </tr>
              <tr>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_input_6.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_ours_6.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_votehmr_6.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_zuo_6.gif"/></td>
              </tr>
            </table>
            <p class="content">
              Qualitative results on <a href="https://www.di.ens.fr/willow/research/surreal/data/">SURREAL</a> dataset which is a synthetic human motion dataset.
              Baselines estimate the parameters for individual frames
              of input, and result in unnatural jittering motion within the
              sequence. On the other hand, our method correctly captures
              temporal correlation and reconstruct meshes with smooth
              motion. 
            </p>
          </div>
        </div>

        <div class="columns">
          <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">Qualitative Results<br><font size="3em">(Human, Real)</font></h2>
          </div>
          <div class="column has-text-justified">
            <table>
              <tr>
                <th style="text-align:center">Input</th>
                <th style="text-align:center">Ours</th>
                <th style="text-align:center">VoteHMR</th>
                <th style="text-align:center">Zuo <i>et al.</i></th>
              </tr>
              <tr>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_input_5.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_ours_5.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_votehmr_5.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_zuo_5.gif"/></td>
              </tr>
              <tr>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_input_0.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_ours_0.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_votehmr_0.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/human_zuo_0.gif"/></td>
              </tr>
            </table>
            <p class="content">
              Qualitative results on <a href="https://ieeexplore.ieee.org/document/6474999">Berkeley MHAD</a> dataset which is a real human motion dataset.
              Even though
              the input point cloud is extremely noisy and the network
              is not fine-tuned to the noisy real data, our model recovers
              the mesh sequence.
            </p>
          </div>
        </div>

        <div class="columns">
          <div class="column is-one-fifth">
            <h2 class="subtitle is-4 is-size-3-mobile has-text-weight-medium publication-keywords">
              Qualitative Results<br><font size="3em">(Hand)</font>
            </h2>
          </div>
          <div class="column has-text-justified">
            <table>
              <tr>
                <th style="text-align:center">Input</th>
                <th style="text-align:center">GT</th>
                <th style="text-align:center">Ours</th>
                <th style="text-align:center">VoteHMR-M</th>
              </tr>
              <tr>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/hand_input_2.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/hand_gt_2.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/hand_ours_2.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/hand_votehmr_2.gif"/></td>
              </tr>
              <tr>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/hand_input_4.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/hand_gt_4.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/hand_ours_4.gif"/></td>
                <td><img src="{{ site.url }}{{ site.baseurl }}/assets/DynamicMeshRecovery/hand_votehmr_4.gif"/></td>
              </tr>
            </table>
            <p class="content">
              Qualitative results on <a href="https://mks0601.github.io/InterHand2.6M/">InterHand2.6M</a> & <a href="https://lmb.informatik.uni-freiburg.de/resources/datasets/HanCo.en.html">HanCo</a> dataset.
              VoteHMR-M is our modification of VoteHMR to fit the MANO hand model.
              In the paper, we include quantitative analysis that our method achieves better result.
            </p>
          </div>
        </div>
      </div>
    </section>
    
    <!-- Content section with centered subtitle -->
    <!--
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
  -->
    <!-- BibTex sectoion -->
    <section class="section">
      <div class="container is-max-desktop">
        <div class="column is-full-width is-centered has-text-centered">
          <h2 class="subtitle is-size-3 has-text-weight-medium publication-keywords">BibTeX</h2>
        </div>
        <div class="box bibtex-box">
          <pre>
@InProceedings{Jang_2023_ICCV,
  author    = {Jang, Hojun and Kim, Minkwan and Bae, Jinseok and Kim, Young Min},
  title     = {Dynamic Mesh Recovery from Partial Point Cloud Sequence},
  booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
  month     = {October},
  year      = {2023},
  pages     = {15074-15084}
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
            <a class="navbar-item" href="https://hojunjang17.github.io/">
              <span class="icon">
                <i class="fas fa-home"></i>
              </span>
            </a>
            <a class="navbar-item" href="https://github.com/hojunJang17">
              <span class="icon">
                <i class="fab fa-github"></i>
              </span>
            </a>
          </div>
          <!--
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
        -->
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

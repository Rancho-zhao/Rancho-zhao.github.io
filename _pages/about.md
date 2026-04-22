---
permalink: /
title: "Yongqiang Zhao"
excerpt: "About me"
layout: home
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

<div class="home-hero">
  <div class="home-hero__photo">
    <img src="{{ '/images/profile.png' | relative_url }}" alt="Portrait of Yongqiang Zhao">
  </div>

  <div class="home-hero__main">
    <h1>Yongqiang Zhao</h1>

    <p class="home-hero__links">
      <a href="{{ '/files/CV_Yongqiang_Zhao.pdf' | relative_url }}">CV</a>
      <span>&amp;</span>
      <a href="{{ site.author.googlescholar }}">Google Scholar</a>
      <span>&amp;</span>
      <a href="https://github.com/{{ site.author.github }}">GitHub</a>
      <span>&amp;</span>
      <a href="{{ site.author.researchgate }}">ResearchGate</a>
      <span>&amp;</span>
      <a href="mailto:{{ site.author.email }}">Email</a>
    </p>

    <p>
      I am a PhD student in the Department of Engineering at
      <a href="https://www.kcl.ac.uk/" target="_blank" rel="noopener noreferrer">King's College London</a>.
      My research lies at the intersection of robotic manipulation, tactile sensing, and robot learning,
      with a particular interest in sim-to-real transfer and perception-driven dexterous interaction.
    </p>

    <p>
      Before joining King's, I received both my Bachelor's and Master's degrees from
      <a href="https://www.seu.edu.cn/" target="_blank" rel="noopener noreferrer">Southeast University</a>.
      This website collects selected papers, projects, and notes from my research journey.
    </p>
  </div>
</div>

<section class="home-section">
  <h2>Recent News</h2>
  <ul>
    <li>[2024.04] Our paper on FOTS was published in <em>IEEE Robotics and Automation Letters</em>.</li>
    <li>[2023.02] Work on tubular object manipulation with tactile sensing appeared in <em>Robotics and Autonomous Systems</em>.</li>
    <li>[2023.01] Our paper on pixel-level domain adaptation for real-to-sim pose estimation was published in <em>IEEE TCDS</em>.</li>
    <li>[Now] I am continuing research on tactile perception, sim-to-real transfer, and dexterous manipulation.</li>
  </ul>
</section>

<section class="home-section">
  <h2>Papers</h2>

  <div class="home-paper">
    <div class="home-paper__media">
      <img src="{{ '/images/fots.gif' | relative_url }}" alt="FOTS preview">
    </div>
    <div class="home-paper__body">
      <div class="home-paper__title">FOTS: A Fast Optical Tactile Simulator for Sim2Real Learning of Tactile-guided Robot Manipulation Skills</div>
      <div class="home-paper__authors"><strong>Y. Zhao</strong>, K. Qian, B. Duan, S. Luo</div>
      <div class="home-paper__venue">IEEE Robotics and Automation Letters, 2024</div>
      <div class="home-paper__links">
        <a class="home-badge" href="https://arxiv.org/abs/2404.19217" target="_blank" rel="noopener noreferrer">Paper</a>
        <a class="home-badge" href="https://github.com/Rancho-zhao/FOTS" target="_blank" rel="noopener noreferrer">Code</a>
        <a class="home-badge" href="https://youtu.be/QUHolBrg4LI" target="_blank" rel="noopener noreferrer">Video</a>
      </div>
    </div>
  </div>

  <div class="home-paper">
    <div class="home-paper__media">
      <img src="{{ '/images/paper_3.gif' | relative_url }}" alt="Tubular manipulation preview">
    </div>
    <div class="home-paper__body">
      <div class="home-paper__title">Skill Generalization of Tubular Object Manipulation with Tactile Sensing and Sim2Real Learning</div>
      <div class="home-paper__authors"><strong>Y. Zhao</strong>, X. Jing, K. Qian, D. Gomes, S. Luo</div>
      <div class="home-paper__venue">Robotics and Autonomous Systems, 2023</div>
      <div class="home-paper__links">
        <a class="home-badge" href="https://www.sciencedirect.com/science/article/abs/pii/S092188902200210X" target="_blank" rel="noopener noreferrer">Paper</a>
        <a class="home-badge" href="https://github.com/Rancho-zhao/Digit_PhongSim" target="_blank" rel="noopener noreferrer">Code</a>
        <a class="home-badge" href="https://youtu.be/NJ9toHPzXXQ" target="_blank" rel="noopener noreferrer">Video</a>
      </div>
    </div>
  </div>

  <div class="home-paper">
    <div class="home-paper__media">
      <img src="{{ '/images/TCDS.png' | relative_url }}" alt="Pose estimation preview">
    </div>
    <div class="home-paper__body">
      <div class="home-paper__title">Pixel-Level Domain Adaptation for Real-to-Sim Object Pose Estimation</div>
      <div class="home-paper__authors">K. Qian, Y. Duan, C. Luo, <strong>Y. Zhao</strong>, X. Jing</div>
      <div class="home-paper__venue">IEEE Transactions on Cognitive and Developmental Systems, 2023</div>
      <div class="home-paper__links">
        <a class="home-badge" href="https://ieeexplore.ieee.org/abstract/document/10018456/" target="_blank" rel="noopener noreferrer">Paper</a>
      </div>
    </div>
  </div>

  <div class="home-paper">
    <div class="home-paper__media">
      <img src="{{ '/images/vitac2023.png' | relative_url }}" alt="ViTac workshop preview">
    </div>
    <div class="home-paper__body">
      <div class="home-paper__title">Unsupervised Adversarial Domain Adaptation for Sim-to-Real Transfer of Tactile Manipulation Skills</div>
      <div class="home-paper__authors">X. Jing, <strong>Y. Zhao</strong>, J. Jiang, B. Duan, K. Qian, S. Luo</div>
      <div class="home-paper__venue">ICRA 2023 ViTac Workshop</div>
      <div class="home-paper__links">
        <a class="home-badge" href="https://shanluo.github.io/ViTacWorkshops/content/ViTac2023_Paper_05.pdf" target="_blank" rel="noopener noreferrer">Paper</a>
      </div>
    </div>
  </div>

  <div class="home-paper">
    <div class="home-paper__media">
      <img src="{{ '/images/apf_rrt.png' | relative_url }}" alt="APF-RRT preview">
    </div>
    <div class="home-paper__body">
      <div class="home-paper__title">Path Planning of UAV Delivery Based on Improved APF-RRT* Algorithm</div>
      <div class="home-paper__authors"><strong>Y. Zhao</strong>, K. Liu, G. Lu, Y. Hu, S. Yuan</div>
      <div class="home-paper__venue">International Conference on Computer Modeling, Simulation and Algorithm, 2020</div>
      <div class="home-paper__links">
        <a class="home-badge" href="https://iopscience.iop.org/article/10.1088/1742-6596/1624/4/042004/pdf" target="_blank" rel="noopener noreferrer">Paper</a>
        <a class="home-badge" href="https://github.com/Rancho-zhao/APF-RRTstar" target="_blank" rel="noopener noreferrer">Code</a>
      </div>
    </div>
  </div>
</section>

<section class="home-section">
  <h2>Selected Projects</h2>

  <div class="home-paper home-paper--project">
    <div class="home-paper__media">
      <img src="{{ '/images/project-sensor/robot_arm.jpg' | relative_url }}" alt="Tactile sensor project">
    </div>
    <div class="home-paper__body">
      <div class="home-paper__title">Reproduction and Improvement of Vision-based Tactile Sensors</div>
      <div class="home-paper__venue">Sensor design, fabrication, and robotic integration</div>
    </div>
  </div>

  <div class="home-paper home-paper--project">
    <div class="home-paper__media">
      <img src="{{ '/images/project-xiaoli/overall.jpg' | relative_url }}" alt="Xiaoli robotic arm project">
    </div>
    <div class="home-paper__body">
      <div class="home-paper__title">Xiaoli: A Robotic Arm for Table Tennis Grasping</div>
      <div class="home-paper__venue">Embedded control, robotic arm design, and autonomous grasping</div>
    </div>
  </div>

  <div class="home-paper home-paper--project">
    <div class="home-paper__media">
      <img src="{{ '/images/project-audio/voice.jpg' | relative_url }}" alt="Audio amplifier project">
    </div>
    <div class="home-paper__body">
      <div class="home-paper__title">A Design of Audio Amplifier</div>
      <div class="home-paper__venue">Circuit design, control, and hardware prototyping</div>
    </div>
  </div>
</section>

<section class="home-section home-section--footer">
  <p>
    This site is now maintained as a single-page academic homepage.
  </p>
</section>

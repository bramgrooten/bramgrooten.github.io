---
layout: page
permalink: /
---


<div class="row justify-content-center align-items-center p-4">
  <div class="col-lg-4 col-md-6 text-center mt-0">

    <img id="profile-pic"
         src="assets/images/bram/bram1.webp" 
         alt="{{ site.title }}" 
         class="rounded-circle shadow-sm" 
         style="width: 200px; height: 200px; object-fit: cover;">

    <p class="text-muted mt-3">
      Postdoc in Deep Learning at the TU Eindhoven
    </p>

    {% include social.html %}

    <p class="text-muted">
      <a href="/assets/pdfs/CV_BramGrooten.pdf" target="_blank">CV.pdf</a>
    </p>

  </div>
</div>


I'm a postdoc in the [AMOR/e](https://amore-labs.github.io/website/) lab at the **TU Eindhoven**, working with [Joaquin Vanschoren](https://joaquinvanschoren.github.io/home/) on vision-language-action models for robotics. In 2026, I am completing my PhD on generalization in deep reinforcement learning, supervised by [Decebal Mocanu](https://www.uni.lu/fstm-en/people/decebal-constantin-mocanu/) and [Mykola Pechenizkiy](https://www.tue.nl/en/research/researchers/mykola-pechenizkiy/). Research interests include robotics, VLAs, RL, generalization, sparse neural networks.

During my PhD, I did an internship at **Sony AI** in the [Gran Turismo](https://www.nature.com/articles/s41586-021-04357-7) team.
We published a paper on large-scale generalization, accepted as an oral at AAAI 2026. Read the paper on [arXiv](https://arxiv.org/pdf/2511.09737)
and see the presentation below.

<div class="col-md-9 col-12 mx-auto">
{% include elements/video.html id="gRp62ZG3Xic" caption="Presentation of the SPARC paper with Sony AI at AAAI, Jan 2026." %}
</div>

In 2023, I visited the **University of Alberta** for 5 months as part of my PhD, joining the 
[Intelligent Robot Learning](https://irll.ca/team/) lab of Matthew Taylor.
See the talk I gave at [Amii](https://www.amii.ca/) in the AI Seminar Series below.

<div class="col-md-9 col-12 mx-auto">
{% include elements/video.html id="oYzQ60xUlDM" caption="Presenting my PhD research at the University of Alberta, August 2023." %}
</div>


In 2021, I finished two masters at the TU Eindhoven called:

- Industrial and Applied Mathematics ([IAM](https://www.tue.nl/en/education/graduate-school/master-industrial-and-applied-mathematics/))
- Science Education and Communication ([SEC](https://www.tue.nl/en/education/graduate-school/master-science-education))

You can find both master theses on [my TU/e page](https://research.tue.nl/en/persons/bram-j-grooten). The thesis for IAM was titled: _Deep Reinforcement Learning for the cooperative card game Hanabi_.

<div class="col-md-9 col-12 mx-auto">
{% include elements/video.html id="5vZ-rrWSivM" caption="Master's thesis presentation, Sept 2021." %}
</div>

For my bachelor of Applied Mathematics, I started my studies at Wentworth Institute of Technology, in Boston, USA. My [bachelor’s thesis](/projects/bachelor-thesis) used graph theory and optimization for a matching assignment problem.

<!-- <div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div> -->

<div class="row">
{% include about/timeline.html %}
</div>

## Contact

<p id="contact-email" class="text-muted mb-0"></p>
<p class="text-muted mb-0">See my <a href="/assets/pdfs/CV_BramGrooten.pdf">CV</a>. Last updated: Feb 2026.</p>
<p class="text-muted mb-0">Here's my <a href="https://scholar.google.com/citations?user=zkYA_KEAAAAJ">Google Scholar</a> page.</p>



<script>
  (function() {
    var u = 'b.grooten';
    var d = 'tue.nl';
    var el = document.getElementById('contact-email');
    if (el) {
      var a = u + '@' + d;
      el.innerHTML = 'Email: <a href="mailto:' + a + '">' + a + '</a>';
    }
  })();

  // To add some variety to the profile picture, we cycle through a set of images each time the page is loaded. 
  const totalImages = 3;
  const storageKey = 'bramImageIndex';
  let currentIndex = sessionStorage.getItem(storageKey);
  if (!currentIndex) {
    currentIndex = 1;
  } else {
    currentIndex = parseInt(currentIndex) + 1;
    if (currentIndex > totalImages) {
      currentIndex = 1;
    }
  }
  sessionStorage.setItem(storageKey, currentIndex);
  if (currentIndex > 1) {
    const imgElement = document.getElementById('profile-pic');
    if (imgElement) {
      imgElement.src = `assets/images/bram/bram${currentIndex}.webp`;
    }
  }
</script>


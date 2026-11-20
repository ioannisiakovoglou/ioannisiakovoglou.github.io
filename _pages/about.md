---
layout: archive
title: "Welcome"
permalink: /
author_profile: true
---

Welcome to my academic website!

I am a postdoctoral researcher working on hyperbolic dynamical systems. I am particularly interested in the interplay between the dynamics of three dimensional flows, topology and combinatorics. 

Here you can find information about my research, publications, teaching activities, talks, and academic work.

## Research

My research focuses on the study of three dimensional Anosov and pseudo-Anosov flows via their bifoliated planes. Currently, I am particularly interested in the project of classification of all pseudo-Anosov flows in dimension 3 by the use of Markov partitions.

## My research in pictures


<div class="research-gallery">

  <figure>
    <img src="{{ '/images/famillemarkov.png' | relative_url }}" alt="Figure 1">
    <figcaption><strong> Figure 1.</strong> A Markovian family associated to the suspension flow of the cat map.</figcaption>
  </figure>

  <figure>
  <img
    src="{{ '/images/markovpartitiongeodflow.jpg' | relative_url }}"
    alt="Figure 2"
    style="display: block; width: 100%; height: 200px; object-fit: contain;"
  >
  <figcaption><strong> Figure 2.</strong> A Markov partition of the geodesic flow on a genus 2 surface (with C. Bonatti).</figcaption>
</figure>

<figure>
  <img
    src="{{ '/images/canonicalmarkovian.png' | relative_url }}"
    alt="Figure 3"
    style="display: block; width: 100%; height: 200px; object-fit: contain;"
  >
  <figcaption><strong>Figure 3.</strong> A canonical Markovian family of a Bonatti-Langevin flow.</figcaption>
</figure>

  <figure>
    <img src="{{ '/images/BLgeomtype.png' | relative_url }}" alt="Figure 4">
    <figcaption><strong>Figure 4.</strong> A geometric type of a Bonatti Langevin flow.</figcaption>
  </figure>

</div>


<figure class="featured-figure">
  <img
    src="{{ '/images/BL.png' | relative_url }}"
    alt="A Bonatti-Langevin flow"
  >
  <figcaption>
    <strong>Figure 5.</strong> My view of the bifoliated plane of a Bonatti-Langevin flow.
  </figcaption>
</figure>




<div id="image-lightbox" class="image-lightbox">
  <button class="lightbox-close" aria-label="Close">&times;</button>
  <img src="" alt="Enlarged research figure">
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const lightbox = document.getElementById("image-lightbox");
  const lightboxImage = lightbox.querySelector("img");
  const closeButton = lightbox.querySelector(".lightbox-close");

  const images = document.querySelectorAll(
    ".research-gallery img, .featured-figure img"
  );

  images.forEach(function (image) {
    image.addEventListener("click", function () {
      lightboxImage.src = image.src;
      lightboxImage.alt = image.alt;
      lightbox.classList.add("active");
    });
  });

  function closeLightbox() {
    lightbox.classList.remove("active");
    lightboxImage.src = "";
  }

  closeButton.addEventListener("click", closeLightbox);

  lightbox.addEventListener("click", function (event) {
    if (event.target === lightbox) {
      closeLightbox();
    }
  });

  document.addEventListener("keydown", function (event) {
    if (event.key === "Escape") {
      closeLightbox();
    }
  });
});
</script>

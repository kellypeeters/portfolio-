<template>
 <div class="row">
            <div class="gallery">
        <figure class="galleryitem galleryitem1">
          <img src="/images/bdo.jpg" class="galleryimg" alt="Image 1">
        </figure>
        <figure class="galleryitem galleryitem2">
          <img src="/images/recept.png" class="galleryimg" alt="Image 2">
        </figure>
        <figure class="galleryitem galleryitem3">
          <img src="/images/hut.png" class="galleryimg" alt="Image 3">
        </figure>
        <figure class="galleryitem galleryitem4">
          <img src="/images/banner.jpg" class="galleryimg" alt="Image 4">
        </figure>
        <figure class="galleryitem galleryitem5">
          <img src="/images/document.jpg" class="galleryimg" alt="Image 5">
        </figure>
        <figure class="galleryitem galleryitem6">
          <img src="/images/mail.jpg" class="galleryimg" alt="Image 6">
        </figure>
      </div>
    </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }

  .galleryimg {
    width: 100%;
    height: 100%;
    object-fit: cover;
    margin-bottom: 1rem;
}

.gallery{
    margin-top: 10rem;
}
}
</style>

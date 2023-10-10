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

    <div class="slider-container">
  <div class="slider">
    <div class="slides">
      <div id="slides__1" class="slide">
        <img src="/images/bookhut.jpg" class="galleryimg" alt="Image 2">
        <a class="slide__prev" href="#slides__4" title="Next"></a>
        <a class="slide__next" href="#slides__2" title="Next"></a>
      </div>
      <div id="slides__2" class="slide">
        <img src="/images/book.jpg" class="galleryimg" alt="Image 2">
        <a class="slide__prev" href="#slides__1" title="Prev"></a>
        <a class="slide__next" href="#slides__3" title="Next"></a>
      </div>
    </div>
  </div> 
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

.slider {
  width: 100%;
  max-width: 600px;
  height: 400px;
  margin: 20px;
  border-radius: 20px;
  overflow: hidden;
  position: relative;
}

.slides {
  display: flex;
  overflow-x: scroll;
  position: relative;
  scroll-behavior: smooth;
  scroll-snap-type: x mandatory;
}

.slide {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-shrink: 0;
  width: 100%;
  height: 400px;
  scroll-snap-align: center;
  margin-right: 0px;
  box-sizing: border-box;
  transform-origin: center center;
  transform: scale(1);
}

.slide a {
  background: none;
  border: none;
}

a.slide__prev,
.slider::before {
  transform: rotate(135deg);
  -webkit-transform: rotate(135deg);
  left: 5%;
}

a.slide__next,
.slider::after {
  transform: rotate(-45deg);
  -webkit-transform: rotate(-45deg);
  right: 5%;
}

.slider::before,
.slider::after,
.slide__prev,
.slide__next {
  position: absolute;
  top: 48%;
  width: 35px;
  height: 35px;
  border: solid black;
  border-width: 0 4px 4px 0;
  padding: 3px;
  box-sizing: border-box;
}

.slider::before,
.slider::after {
  content: "";
  z-index: 1;
  background: none;
  pointer-events: none;
}
}
</style>

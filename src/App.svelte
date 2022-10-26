<script>
  import { images } from "./imageData.js";
  import Slide from "./components/Slideshow.svelte";
  import Caption from "./components/Caption.svelte";
  //   let slideNo;
  //   let totalSlide;
  //   let varx;
  let imageShowIndex = 0;
</script>

<div class="container" />
{#each images as { id, name, imgurl }}
  <Slide
    image={imgurl}
    altTag={name}
    imageShowing={id === imageShowIndex}
    slideNo={id + 1}
    totalSlide={images.length}
  />
{/each}

<Caption 
    caption ={images[imageShowIndex].name}

/>

<style>
</style>

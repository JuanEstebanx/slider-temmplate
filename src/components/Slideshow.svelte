<script>
  export let slideNo;
  export let totalSlide;
  export let image;
  export let altTag;
  export let attr;
  export let imageShowing;
</script>

<div class="mySlides" class:show={imageShowing}>
  <div class="numbertext">{slideNo} / {totalSlide}</div>
  <img src={image} alt={altTag} title={attr} />
</div>

<style>
  .mySlides {
    display: none;
  }
  img {
    width: 100%;
  }
  .show {
    display: block;
  }
</style>

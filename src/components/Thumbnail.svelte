<script>
  export let thumbImg;
  export let altTag;
</script>

  <div class="thumbnails-col">
    <img
      class="sample cursor"
      src={thumbImg}
      style="width:100%"
      alt={altTag}
      on:click
      
    />
  </div>

<style>
  
  .sample {
    opacity: 0.6;
  }
  .active,
  .sample:hover {
    opacity: 1;
  }

  /* Six columns side by side */
  .thumbnails-col {
    float: left;
    width: 16.66%;
  }
</style>

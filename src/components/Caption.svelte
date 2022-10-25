<script>
  import { createEventDispatcher } from "svelte";
  export let caption;

  const dispatch = createEventDispatcher();
</script>

<!-- Image text -->
<div class="caption-container">
  <p id="caption">{caption}</p>
</div>

<!-- Next and previous buttons -->
<a href="#hola" class="prev" on:click={() => dispatch("prevClic")}>&#10094;</a>
<a href="#hola" class="next" on:click={() => dispatch("nextClic")}>&#10095;</a>

<style>
  /* Container for image text */
  .caption-container {
    text-align: center;
    background-color: #222;
    padding: 2px 16px;
    color: white;
  }

  /* Next & previous buttons */
  .next {
    margin-right: 8px;
  }
  .prev,
  .next {
    cursor: pointer;
    position: absolute;
    top: 200px;
    width: auto;
    padding: 16px;
    margin-top: -50px;
    color: white;
    font-weight: bold;
    font-size: 20px;
    border-radius: 0 3px 3px 0;
    user-select: none;
    -webkit-user-select: none;
  }

  /* Position the "next button" to the right */
  .next {
    right: 0;
    border-radius: 3px 0 0 3px;
  }

  /* On hover, add a black background color with a little bit see-through */
  .prev:hover,
  .next:hover {
    /* background-color: rgba(0, 0, 0, 0.8); */
    background-color: red;
  }
</style>

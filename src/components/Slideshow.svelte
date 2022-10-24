<script>
    export let image;
    export let attr;
    export let altTag;
    export let totalSlides;
    export let slideNo;
    export let imageShowing;
</script>

<!-- Full-width images with number text -->
<div class="mySlides" class:show={imageShowing}>
    <div class="numbertext">{slideNo} / {totalSlides}</div>
    <img src={image} title={attr} alt={altTag} />
</div>

<style>
    /* Hide the images by default */
    .mySlides {
        display: none;
    }
    /* Number text (1/3 etc) */
    .numbertext {
        color: #f2f2f2;
        font-size: 12px;
        padding: 8px 12px;
        position: absolute;
        top: 0;
    }
    img {
        width: 100%;
    }
    .show{
        display: block;
    }
</style>

<script>
    import { images } from "./imageData.js";
    let slideNo;
    let totalSlide;
    let varx;
        
    let  imageurl = "https://wallpapercave.com/wp/fDIESuJ.jpg";

</script>

<div class="container">
    <!-- Full-width images with number text -->
    <div class="mySlides">
        <div class="numbertext">{slideNo} / {totalSlide}</div>
        <img src={images as imgurl} alt={varx} style="width:100%" />}
    </div>
</div>

<style>
    .mySlides {
        /* display: none; */
    }
</style>

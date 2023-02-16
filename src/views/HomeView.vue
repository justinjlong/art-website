<template>
  <div class="home">
    <div class="first-row row mt-4">
      <div>
        <h6 class="text-center">{{ aboutDescription }}</h6>
        <hr>
      </div>
    </div>
    <div class="container gallery-container">
    <div class="tz-gallery">

        <div class="row">

            <div class="col-sm-6 col-md-4 ">
                <div class="thumbnail">
                    <!-- <a class="lightbox" href="@/assets/art/wooly_worm.jpg"> -->
                        <img src="@/assets/art/wooly_worm.jpg" alt="Park" width="100%">
                    <!-- </a> -->
                    <div class="caption">
                        <h3>Appalachian History</h3>
                        <p>Inspired by folk history and tradition.</p>
                    </div>
                </div>
            </div>
             <div class="col-sm-6 col-md-4">
                <div class="thumbnail">
                    <!-- <a class="lightbox" href="@/assets/art/104k_buck.jpg"> -->
                        <img src="@/assets/art/104k_buck.jpg" alt="Park" width="100%">
                    <!-- </a> -->
                    <div class="caption">
                        <h3>The Natural World</h3>
                        <p>Large scale ball point pen drawings.</p>
                    </div>
                </div>
            </div>
            <div class="col-sm-6 col-md-4">
                <div class="thumbnail">
                    <!-- <a class="lightbox" href="@/assets/art/wood.jpg"> -->
                        <img src="@/assets/art/west.jpg" alt="Park" width="100%">
                    <!-- </a> -->
                    <div class="caption">
                        <h3>Water Colors</h3>
                        <p>Pen, ink, water, and sometimes color.</p>
                    </div>
                </div>
            </div>
           
            
        </div>

    </div> 
    </div>
  </div>
</template>

<script lang="ts">
export default {
  data() {
      return {
         welcomeText: "Welcome.",
         aboutDescription: "I am a Pittsburgh based artist interested in exploring and reimagining the natural world though folk history and textures."
      }
    }
}
</script>


<style>
@media (min-width: 1024px) {
  .home {
    min-height: 80vh;
    display: flex;
    flex-direction: column !important;
    align-items: center;
    justify-content: center;
  }
}

.first-row {
  padding-top: 1%;
}

.gallery-container h1 {
    text-align: center;
    margin-top: 70px;
    font-family: 'Droid Sans', sans-serif;
    font-weight: bold;
    color: #58595a;
}

.gallery-container p.page-description {
    text-align: center;
    margin: 30px auto;
    font-size: 18px;
    color: #85878c;
}


.tz-gallery {
    padding: 40px;
}

.tz-gallery .thumbnail {
    padding: 0;
    margin-bottom: 30px;
    border: none;
}

.tz-gallery img {
    border-radius: 2px;
}

.tz-gallery .caption{
    padding: 26px 30px;
    text-align: center;
}

.tz-gallery .caption h3 {
    font-size: 14px;
    font-weight: bold;
    margin-top: 0;
}

.tz-gallery .caption p {
    font-size: 12px;
    color: #7b7d7d;
    margin: 0;
}

</style>
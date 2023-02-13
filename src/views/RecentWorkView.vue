<template>
  <div class="home">
      <div class="container">
      <div class="row">
          <div class="col-12">
            <img src="@/assets/art/104k_buck.jpg" width="600" class="ml-4 ">
            <img src="@/assets/art/deerframe.jpg" width="400" class=" mx-4 mb-2">
          </div>
      </div>
      <div class="row">
          <div class="col-2">
            
          </div>
          <div class="col-10"> 
                <img src="@/assets/art/cat_deer.jpg" width="200" class="mx-4" style="align-items: left">
                <img src="@/assets/art/fishdeer.jpg" width="700" class="mt-1 mx-5">
          </div>
      </div>
      </div>
      
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .home {
    min-height: 90vh;
    display: flex;
    flex-direction: row !important;
    align-items: center;
    justify-content: center;
  }
}

img {
  border: 5px solid rgba(181, 201, 187, 0.6) ;
}

</style>
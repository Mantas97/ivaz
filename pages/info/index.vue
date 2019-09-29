<template>
<!-- <b-container fluid>
  <b-row align-v="center" class="justify-content-center">

    <b-col sm="10" offset-sm="1">
      <h5>bybis</h5>
    </b-col>

  </b-row>
</b-container> -->
 <div class="center-screen">
     <div class="bybis">
         <h5>adsasdasd</h5>
         <h6>adsasdasd</h6>
     </div>
 </div>

</template>




<style lang="scss" scoped>

$background-color: #F1F9FF;

.center-screen {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  min-height: 100vh;
  background-color: $background-color;

  .bybis{
      width: 80%;
      background-color: red;
  }
}

.container-fluid{
    background-color: $background-color;
    height: 100vh;

    > .row{
        // width: 80%;
        height: 100%;
    }

    // div{
    //     display: contents;
    //     margin: auto;
    //     background-color: white;
    // }
}




</style>
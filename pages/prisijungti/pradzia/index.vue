<template>
<section>

    <b-container fluid class="i-start-title ">
        <b-row align-v="end" class="justify-content-center">
            <h4>Instrukcijos</h4>
        </b-row>
    </b-container>


    <b-container fluid class="i-start-content">
        <h5>Image</h5>
    </b-container>



    <b-container fluid class="i-start-text">
        <b-row align-v="start" class="justify-content-center">
            <div class="i-start-textdiv">
                <h5>Main Title</h5>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod.</p>
            </div>
        </b-row>
    </b-container>

    <b-container fluid class="i-button-container">
        <b-row align-v="start" class="justify-content-center">
            <nuxt-link to="#" >
                <b-button class="i-button-submit">Pradėti</b-button>
            </nuxt-link>
        </b-row>
    </b-container>


</section>
</template>




<style lang="scss" scoped>

$primary-color: #2699FB;



.i-start-title{
    height: 15vh;

    h4{
        margin-bottom: 1rem;
        text-transform: uppercase;
        font-weight: 700;
    }
}
.i-start-title .row, .i-start-text .row{
    height: 100%;
}
h4, h5, p{
    color: $primary-color;
}


.i-start-content{
    background-color: $primary-color;
    height: 50vh;
}


.i-start-text{
    height: 20vh;

    .i-start-textdiv{
        width: 90%;
        text-align: center;
        padding-top: 1rem; 
    }

    .i-start-text h5{
        font-weight: 700;
    }
}




</style>
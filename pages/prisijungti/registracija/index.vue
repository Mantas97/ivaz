<template>
<section>

    <b-container fluid class="i-signup-title">
        <b-row align-v="end" class="justify-content-center">
            <h2>Simple I.VAZ</h2>
        </b-row>
    </b-container>


    <b-container fluid class="i-signup-content">
        <b-row align-v="center" class="justify-content-center">
            <div class="i-signup-inputs">
                <b-form-input placeholder="El. paštas"></b-form-input>
                <b-form-input placeholder="Slaptažodis"></b-form-input>
            </div>
        </b-row>
    </b-container>


<!-- class="justify-content-center" -->
    <b-container fluid class="i-button-container">
        <b-row align-v="start" class="justify-content-center">
            <nuxt-link to="/prisijungti/pradzia" >
                <b-button class="i-button-submit">Prisijungti</b-button>
            </nuxt-link>
        </b-row>
    </b-container>


</section>
</template>

<style lang="scss" scoped>
$primary-color: #2699FB;
$secondary-color: #BCE0FD;


.i-signup-title{
    background-color: $primary-color;
    height: 22vh;

    .row{
        height: 100%;
    }
    h2{
        color: white;
        margin-bottom: 1rem;
        font-family: 'RobotoRegular';
    }
}




.i-signup-content{
    height: 63vh;

    .row{
        height: 100%;
    }

    .i-signup-inputs{
        width: 80%;
        margin-top: -2rem;

        .form-control:first-child{
            margin-bottom: 2rem;
        }

        input[type="text"].form-control {
            height: calc(2em + 0.75rem + 2px);
            font-size: 1.1rem;
            font-weight: 600;
            border-radius: 1.5rem;
            border: 2px solid #80bdff;
            color: $primary-color;
        }

        input[type="text"].form-control::placeholder { /* Chrome, Firefox, Opera, Safari 10.1+ */
            color: #80bdff;
            opacity: 1; /* Firefox */
        }
        input[type="text"].form-control::-ms-input-placeholder { /* Microsoft Edge */
            color: #80bdff;
        }
    }
}


</style>
<template>
<section>

    <b-container class="bv-example-row bv-example-row-flex-cols">
        <b-row align-v="start">
            <b-col>One of three columns</b-col>
            <b-col>One of three columns</b-col>
            <b-col>One of three columns</b-col>
        </b-row>

        <b-row align-v="center">
            <b-col>One of three columns</b-col>
            <b-col>One of three columns</b-col>
            <b-col>One of three columns</b-col>
        </b-row>

        <b-row align-v="end">
            <b-col>One of three columns</b-col>
            <b-col>One of three columns</b-col>
            <b-col>One of three columns</b-col>
        </b-row>
    </b-container>

</section>
</template>

<style lang="scss">
$primary-color: #2699FB;


html, body{
    overflow: hidden;
}
section{
    height: 100vh;
}
.i-title-box{
    background-color: $primary-color;
    min-height: 22%;
    // align-items: flex-end;
}

</style>
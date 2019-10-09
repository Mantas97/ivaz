<template>
 <div class="i-center-screen">
     <div class="i-centered-div">

       <doc-registered v-if="show === 'DocRegistered'"/>
       <no-connection v-else-if="show === 'NoConnection'"/>
       <doc-sent v-else-if="show === 'DocSent'"/>
       <error v-else-if="show === 'Error'"/>


        <!-- <p>
          Pateikti važtaraštį? <br>
          Patvirtinu, kad informacija teisinga.
        </p> -->

        <!-- <div class="i-two-buttons">
          <div class="i-accept-button">
            <i class="material-icons">check</i>
          </div>
          <div class="i-deny-button">
            <i class="material-icons">close</i>
          </div>
        </div> -->
     </div>
 </div>
</template>


<script>
import DocRegistered from '~/components/info-components/DocRegistered';
import NoConnection from '~/components/info-components/NoConnection';
import DocSent from '~/components/info-components/DocSent';
import Error from '~/components/info-components/Error';
export default {
  components: {
    DocRegistered,
    NoConnection,
    DocSent,
    Error
  },  
  data: function () {
  return {
    show: 'Error'
    }
  }
}
</script>








<style lang="scss">

$background-color: #F1F9FF;
$text-color: #2699FB;

.i-center-screen {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  min-height: 100vh;
  background-color: $background-color;

  .i-centered-div{
    width: 80%;
    background-color: white;
    -webkit-box-shadow: 3px 16px 30px 7px rgba(210,233,252,1);
    -moz-box-shadow: 3px 16px 30px 7px rgba(210,233,252,1);
    box-shadow: 3px 16px 30px 7px rgba(210,233,252,1);
    padding: 2rem;
    color: $text-color;

    img{
      width: 65%;
      margin: 4rem auto 3rem;
    }

    h6, a{
      font-weight: 700;
      font-size: 1.2rem;
    }

    h6{
      margin-bottom: 1rem;
    }

    a{
      color: $text-color;
    }
    a:active{
      text-decoration: underline;
      color: #1d7dce;
    }


    div.i-accept-button, div.i-deny-button{
      background-color: $background-color;
      height: 4rem;
      width: 4rem;
      border-radius: 50%;
      margin: 3rem auto 0rem;
      vertical-align: middle;
      display: flex;
      justify-content: center;
      align-items: center; 
      cursor: pointer;
    }
    div.i-accept-button:active, div.i-deny-button:active{
      background-color: $text-color !important;
      color: white !important;
    }

    div.i-two-buttons{
      margin-top: 2rem;

      div.i-accept-button, div.i-deny-button{
        display: inline-flex;
      }
      div.i-accept-button{
        margin: 0 1rem 0 0;
      }
      div.i-deny-button{
        background-color: white;
        border: 2px solid $background-color;
        margin: 0;
      }
    }

    span.i-important{
      font-weight: 700;
      text-transform: uppercase;
    }

  }
}

// .container-fluid{
//     background-color: $background-color;
//     height: 100vh;

//     > .row{
//         // width: 80%;
//         height: 100%;
//     }

//     // div{
//     //     display: contents;
//     //     margin: auto;
//     //     background-color: white;
//     // }
// }




</style>
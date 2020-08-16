<template>
    <div class="question-box">
  <b-jumbotron>
    <template v-slot:header></template>
     {{currentQuestion.question}}
    <template v-slot:lead>

     
    </template>

    <hr class="my-4">
<p>
List of answer
</p>
    

    <b-button variant="primary" href="#">Submit</b-button>
    <b-button @click="next" variant="success" >Next</b-button>
  </b-jumbotron>
</div>
</template>

<script>
export default {
   props:{
      currentQuestion:Object,
      next:Function
   }
}
</script>
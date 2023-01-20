<script>
export default{
  data(){
    return{
      numberClass:"number",
      count: 0
    }
  },
  methods : {
    increment(){
      this.count++;
    }
  }
}
</script>

<template>
  <h1 v-bind:class="numberClass">{{ count }}</h1>
  <h3>vue로 확인하는 웹페이지 입니다. 아래 버튼을 누르면 값이 1씩 증가합니다</h3>
  <button v-on:click="increment" >1+</button>
</template>

<style>
.number{
  color: red;
}
</style>
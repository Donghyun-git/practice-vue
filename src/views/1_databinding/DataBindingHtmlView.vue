<template>
  <div>
    {{ htmlString }} {{ coment }} 
    <div v-html="htmlString"></div> <!--v-directive 로 데이터 바인딩 하면 innerHTML로 들어감.-->
  </div>
</template>

<script>
export default {
  data() {
    return {
      htmlString: '<p style="color:red;">html 데이터 바인딩</p>',
      coment: '그대로 출력됩니다.'
    }
  }
}
</script>

<style scoped>

</style>

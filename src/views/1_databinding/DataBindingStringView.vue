<template>
    <div>
        <h1> {{ userName }}</h1>
        <p> {{ message }} </p>
    </div>
</template>
<script>
export default {
  data() {
    return {
      userName: '3/14 인증',
      message: '해결완료'
    }
  }
}
</script>
<style scoped>

</style>

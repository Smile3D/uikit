<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <btn
      additionalClass="btn--bg-primary"
      textBtn="primary text"
      textColor="btn--color-text-primary"
    ></btn>
    <btn
      additionalClass="btn--bg-secondary"
      textBtn="secondary text"
      textColor="btn--color-text-primary"
    ></btn>
    <btn
      additionalClass="btn--outline"
      textBtn="secondary text"
      textColor="btn--color-text-secondary"
    ></btn>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld'
import Btn from '@/components/Buttons/Btn'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    Btn
  }
}
</script>

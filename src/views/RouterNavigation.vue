<template>
  <button type="button" @click="getRoute">getRoute</button>
  <button type="button" @click="push">Push</button>
  <button type="button" @click="replace">Replace</button>
  <button type="button" @click="go">Go</button>
  <button type="button" @click="back">back</button>
  <button type="button" @click="forward">forward</button>
  <br>
  <button type="button" @click="addRoute">新增路由</button>
</template>

<script>
export default {
  methods: {
    getRoute () {
      console.log(this.$route)
      console.log(this.$router)
    },
    push () {
      this.$router.push({ name: 'About' })
    },
    replace () {
      this.$router.replace('/newpage/a')
    },
    go () {
      this.$router.go(-2)
    },
    addRoute () {
      this.$router.addRoute({
        path: '/newAbout',
        name: 'newAbout',
        component: () => import('./About.vue')
      })
    },
    forward () {
      this.$router.forward()
    },
    back () {
      this.$router.back()
    }
  }
}
</script>

<template>
  <div>
    班级 {{count}}
  </div>
</template>

<script>
  import {mapState, mapGetters} from 'vuex'

  export default {

    data () {
      return {
        motto: 'Hello miniprograme'
      }
    },

    components: {},

    computed: {
      ...mapState([
        'count'
      ]),
      ...mapGetters({'countNum': 'getCount'})
    },

    methods: {},

    created () {
      // let app = getApp()
    }
  }
</script>

<style lang="scss" scoped>
</style>

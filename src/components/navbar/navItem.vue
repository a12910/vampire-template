<script>
  import {mapState, mapMutations} from 'vuex';

  export default {
    name: 'nav-item',
    props: ['to', 'icon'],
    beforeMount() {

    },
    mounted() {

    },
    destroyed() {

    },
    computed: {
      ...mapState({}),
    },
    methods: {
      ...mapMutations({}),
    },
  };

</script>

<style scoped lang="vcss">

</style>

<template>
  <router-link :id="$options.name" :class="$options.name" class="navbar-item" :to="to">
    <span class="icon"><i class="fas" :class="icon"></i></span>
    <span><slot></slot></span>
  </router-link>
</template>

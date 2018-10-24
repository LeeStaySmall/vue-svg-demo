<template>
    <div class="svg-demo">
        <ul>
            <li v-for="(name, index) in svgName" :key="index">
                <svg-icon :iconClass="name"></svg-icon>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'svgDemo',
  data () {
    return {
      svgName: ['user', 'password', 'email']
    }
  }
}
</script>

<style lang="scss">
    .svg-demo{
        text-align: center;
        ul, li{
            list-style: none;
            padding: 0;
            margin: 0;
            line-height: 2;
        }
    }
</style>

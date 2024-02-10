<template>
    <div class="header">
        <div>
            <img src="../../assets/images/Logo.png" alt="">
        </div>
        <div class="tel">
            +7 987 654 32-10
        </div>
    </div>
</template>

<script>
// import { ref } from 'vue'

export default {
  name: 'HeaderComponent',
  components: {
  },
  props: {
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>
.header {
    display: flex;
    height: 60px;
    // width: 100%;
    padding: 13px 70px;
    justify-content: space-between;
    align-items: center;
    gap: 10%;
    background-color: #3278FF;
    margin-bottom: 235px;
}

.tel {
    color: #FFF;
    font-family: Roboto;
    font-size: 22px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}
</style>

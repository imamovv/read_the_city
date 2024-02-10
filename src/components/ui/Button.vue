<template>
    <div>
      <button class="buttonBuy">Купить</button>
    </div>
  </template>

<script>
// import { ref } from 'vue'

export default {
  name: 'ButtonBuy',
  components: {
  },
  props: {
  },
  setup () {
  }
}
</script>

  <style lang="scss" scoped>
  .buttonBuy {
    display: inline-flex;
    padding: 6px 38px;
    justify-content: center;
    align-items: center;
    gap: 10px;
    border-radius: 7px;
    background-color: #3278FF;
    color: #FFFFFF;
    font-family: Roboto;
    font-size: 20px;
    font-style: normal;
    font-weight: 500;
    line-height: 22px;
    /* 110% */
    letter-spacing: -0.4px;
    margin-top: 34px;
  }
  </style>

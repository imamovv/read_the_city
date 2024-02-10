<template>
    <div class="bookInfo">
        <h2 class="card__title">{{ title }}</h2>
        <h3 class="card__author">{{ author }}</h3>
    </div>
</template>

<script>
// import { ref } from 'vue'

export default {
  name: 'BookInfoComponent',
  components: {
  },
  props: {
    title: {
      type: String,
      default: 'Имя книги'
    },
    author: {
      type: String,
      default: 'Имя автора'
    }
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>
.bookInfo {
    display: inline-flex;
    flex-direction: column;
    align-items: center;
    gap: 14px;
}

.card__title {
    color: var(--, #000);
    text-align: center;
    font-family: Roboto;
    font-size: 24px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    width: 90%;
}

.card__author {
    color: var(--, #000);
    font-family: Roboto;
    font-size: 20px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
</style>

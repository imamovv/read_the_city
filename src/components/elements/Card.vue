<template>
  <div class="card">
      <img class="card__image" :src="imageSource" alt="image.png">
      <div class="card__info">
          <BookInfoComponent :title="title" :author="author" />
      </div>
      <div class="buttonBuy">
          <ButtonBuyVue />
      </div>
  </div>
</template>

<script>
import ButtonBuyVue from '../ui/Button.vue'
import BookInfoComponent from '@/components/elements/CardInfoComponent.vue'
// import { ref } from 'vue'

export default {
  name: 'BookCard',
  components: {
    ButtonBuyVue,
    BookInfoComponent
  },
  props: {
    title: {
      type: String,
      default: 'Имя книги'
    },
    author: {
      type: String,
      default: 'Имя автора'
    },
    imageSource: {
      type: String,
      default: 'default'
    }
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>
.card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  border-radius: 10px;
  background: var(--, #FFF);
  box-shadow: 1px 1px 4px 0px rgba(0, 0, 0, 0.30);
  width: 330px;
  height: 490px;
}

.buttonBuy {
  display: flex;
  flex-direction: column;
}

.card__info {
  margin-top: 16px;
}
</style>

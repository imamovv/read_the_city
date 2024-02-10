<template>

  <main class="main">
  <HeaderComponent />
    <div class="cardFrame">
      <Card v-for="(bookData, index) in bookCardData" v-bind:key="index" :author="bookData.author"
        :title="bookData.title" :imageSource="bookData.imageSource" />
    </div>
  </main>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import Card from '@/components/elements/Card.vue'
import HeaderComponent from '@/components/blocks/HeaderComponent.vue'

export default {
  name: 'MainPage',
  components: {
    Card,
    HeaderComponent
  },
  data () {
    return {
      bookCardData: [
        {
          author: 'Франк Экстанази',
          title: 'Skyrim. Как продать игру 10 раз',
          imageSource: require('@/assets/images/image1.png')
        },
        {
          author: 'Сергей Анисимов',
          title: 'Поисковое продвижение сайтов',
          imageSource: require('@/assets/images/image2.png')
        },
        {
          author: 'Татьяна Магарина',
          title: 'Английский для дизайнеров',
          imageSource: require('@/assets/images/image3.png')
        },
        {
          author: 'Шон Адамс',
          title: 'Дизайн и цвет. Практикум',
          imageSource: require('@/assets/images/image4.png')
        }
      ]
    }
  },
  props: {

  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>
.cardFrame {
  display: flex;
  align-items: flex-start;
  gap: 30px;
  justify-content: center;
}
.header {
  display: flex;
  height: 60px;
  padding: 13px 70px;
  justify-content: space-between;
  align-items: center;
  gap: 10%;
  background-color: #3278FF;
  margin-bottom: 180px;
}
</style>

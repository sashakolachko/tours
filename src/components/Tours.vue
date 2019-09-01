<template lang="html">
<div class="tours-container">
  <div class="tours-container__item"  v-for="tour in tourList">
    <Tour :imgUrl="tour.imgUrl" :date="tour.date" :destination="tour.destination" :description="tour.description" />
  </div>
</div>
</template>

<script>
import Tour from './Tour.vue';
export default {
  name: 'Tours',
  components: {
    Tour
  },
  data: () => {
    return {
      tourList: [{
          imgUrl: require('../assets/newyork.jpg'),
          date: "10.09.2019",
          destination: "New York USA",
          description: "New York State has it all – booming metropolises, majestic waterfalls, mountains, wine country, chicken wings. Yes, NYC is a magnet for tourists, but an exploration of the rest of the state can be equally thrilling.."
        },
        {
          imgUrl: require('../assets/greece.jpg'),
          date: "12.09.2019",
          destination: "Santorini Greece",
          description: "Santorini is considered to be the most sought after place for a romantic getaway in Greece, since there are not many places in the world where you can enjoy exquisitely clear waters while perched on the rim of a massive active volcano in the middle of the sea!"
        },
        {
          imgUrl: require('../assets/prague.jpg'),
          date: "29.10.2019",
          destination: "Prague Czech Republic",
          description: "Prague is a political, cultural and economic centre of central Europe complete with a rich history. Founded during the Romanesque and flourishing by the Gothic, Renaissance and Baroque eras, Prague was the capital of the Kingdom of Bohemia and the main residence of several Holy Roman Emperors, most notably of Charles IV."
        },
        {
          imgUrl: require('../assets/kioto.jpg'),
          date: "21.10.2019",
          destination: "Kyoto Japan",
          description: "Kyoto is considered the cultural capital of Japan and a major tourist destination. It is home to numerous Buddhist temples, Shinto shrines, palaces and gardens, many of which are listed collectively by UNESCO as a World Heritage Site."
        },
        {
          imgUrl: require('../assets/london.jpg'),
          date: "13.11.2019",
          destination: "London United Kingdom",
          description: "London is considered to be one of the world's most important global cities and has been termed the world's most powerful, most desirable, most influential, most visited, most expensive, innovative, sustainable, most investment friendly, most popular for work, and the most vegetarian-friendly city in the world."
        },
        {
          imgUrl: require('../assets/venice.jpg'),
          date: "02.12.2019",
          destination: "Venice Italy",
          description: "Venice is one of our favorite spots in Italy. Why? It is small and compact, perfect to be explored with just a few days time. Venice is romantic, historic, and gorgeous. The canals, the gondolas, the architecture, the colorful towns of Murano and Burano…"
        }
      ]

    }
  }
}
</script>

<style lang="scss" scoped>
.tours-container {
    width: 80vw;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    margin-top: 50px;
    margin-bottom: 50px;
    &__item {
        margin-top: 20px;
    }
}
</style>

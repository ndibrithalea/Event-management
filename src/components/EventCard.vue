<template>
  <div class="card mb-4 text-white">
        <img class="card-img" :src="event.featuredImage" alt="Card image">
        <div class="card-img-overlay">
            <h5 class="card-title my-5">{{event.name}}</h5>
            <p class="card-text">{{event.description}}</p>
            <small class="event-date">{{event.date}}</small>
        </div>
    </div>
</template>
<script>
  export default {
    props: [
      'event'
    ]
  }
</script>
<style lang="scss" scoped>
.card{
  width: 350px !important;
}
  .event-date {
    background-color: #28a745;
    color: #FFF;
    font-size: .75em;
    padding: 2px 10px;
    position: absolute;
    top: 0;
    right: 0;
  }
  .card-img-overlay{
      background-color: #1613132f;
  }
  .card-img{
      height: 300px;
      width: inherit;
  }
</style>
<template>
  <div class="events container">
    <h2 class="mt-5 mb-3 text-bold"> Check out our upcoming events</h2>
        <div class="row">
          <div v-for="even in events" :event="even" :key="even.id">        
            <div class="col-md-4">
                <router-link :to="'/event/' + even.id">
                    <EventCard :event="even" />
                </router-link>
              </div>
          </div>
        </div>
    </div>
</template>

<script>
  import EventCard from '@/components/EventCard';
  export default {
    name: 'EventsList',
    components : {
      EventCard
    },
    data(){
        return {
            event: {},
            events:[
                {
                id: 1,
                name: 'Charity Ball',
                category: 'Fundraising',
                description: 'Spend an elegant night of dinner and dancing with us as we raise money for our new rescue farm.',
                featuredImage: 'https://placekitten.com/400/300',
                images: [
                    'https://placekitten.com/400/400',
                    'https://placekitten.com/400/400',
                    'https://placekitten.com/400/400',
                ],
                location: '1234 Fancy Ave',
                date: '12-25-2019',
                time: '11:30'
                },
                              {
                id: 4,
                name: 'Charity Ball',
                category: 'Fundraising',
                description: 'Spend an elegant night of dinner and dancing with us as we raise money for our new rescue farm.',
                featuredImage: 'https://placekitten.com/400/500',
                images: [
                    'https://placekitten.com/400/400',
                    'https://placekitten.com/400/400',
                    'https://placekitten.com/400/400',
                ],
                location: '1234 Fancy Ave',
                date: '12-25-2019',
                time: '11:30'
                },
                              {
                id: 3,
                name: 'Charity Ball',
                category: 'Fundraising',
                description: 'Spend an elegant night of dinner and dancing with us as we raise money for our new rescue farm.',
                featuredImage: 'https://placekitten.com/500/500',
                images: [
                    'https://placekitten.com/400/400',
                    'https://placekitten.com/400/400',
                    'https://placekitten.com/400/400',
                ],
                location: '1234 Fancy Ave',
                date: '12-25-2019',
                time: '11:30'
                },
                {
                id: 2,
                name: 'Rescue Center Goods Drive',
                category: 'Adoptions',
                description: 'Come to our donation drive to help us replenish our stock of pet food, toys, bedding, etc. We will have live bands, games, food trucks, and much more.',
                featuredImage: 'https://placekitten.com/500/600',
                images: [
                    'https://placekitten.com/500/500'
                ],
                location: '1234 Dog Alley',
                date: '11-21-2019',
                time: '12:00'
                }
            ]
        }
    }
  }
</script>

<style lang="scss" scoped>
 
</style>
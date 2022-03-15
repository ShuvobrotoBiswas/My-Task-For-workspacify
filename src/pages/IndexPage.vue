<template>
   <div class="q-pa-md" >
    <div class="row">
      <div  class="col">
       <q-btn dense rounded icon="event_available">
       </q-btn>
        Total Reserve <br>
        4,500
      </div>
      <div class="col">
       <q-btn dense rounded icon="monetization_on">
       </q-btn>
        Total Revenue <br>
        $13,008
      </div>
      <div class="col">
       <q-btn dense rounded icon="drive_eta">
       </q-btn>
        Total Cars <br>
        110
      </div>
       <div class="col">
       <q-btn dense rounded icon="people">
       </q-btn>
        Total Customers <br>
        200
      </div>
    </div>
    <div class="row">
      <div  class="col">
       <div>
      <apexchart width="500" type="line" :options="options" :series="series"></apexchart>
    </div>
      </div>
    </div>
    <div class="row">
      <div  class="col-9">
      <div class="q-pa-md">

    <div class="row">
      <div class="col-5">
        <div class="row">
          <div class="col-8 col-sm-6">
             <q-img src="https://hips.hearstapps.com/hmg-prod.s3.amazonaws.com/images/2021-sti-and-wrx-1647038410.jpg?crop=0.478xw:0.525xh;0.0901xw,0.244xh&resize=640:*">
        </q-img>
          </div>
          <div class="col-4 col-sm-6">
           <div class="text-h6">
           BMW GH2890
           </div>
           <div class="text-h7">
           BMW GH2890
           </div>
           <div>
            Size: Small
           </div>
          </div>
        </div>
      </div>
      <div class="col">
      End <br> 11:00 PM 08 Mar 22 <br>
      Start <br> 10:00 AM 03 Mar 22
      </div>
      <div class="col"> <br>
        <q-btn color="green-13">
        Accept
        </q-btn> <br> <br> <br>
        <q-btn color="deep-orange-3">
        Decline
        </q-btn>
      </div>
      <div class="col">
        <div class="text-h6">
        ID #4500
        </div> <br>
      <q-btn color="yellow">
        Pending
        </q-btn>
      </div>
    </div>

    <div class="row">
      <div class="col-5">
        <div class="row">
          <div class="col-8 col-sm-6">
             <q-img src="https://i.ytimg.com/vi/ekgUjyWe1Yc/maxresdefault.jpg">
        </q-img>
          </div>
          <div class="col-4 col-sm-6">
           <div class="text-h6">
           BMW GH2890
           </div>
           <div class="text-h7">
           BMW GH2890
           </div>
           <div>
            Size: Small
           </div>
          </div>
        </div>
      </div>
      <div class="col">
      End <br> 11:00 PM 08 Mar 22 <br>
      Start <br> 10:00 AM 03 Mar 22
      </div>
      <div class="col-2">
        <div class="text-h6">
        ID #4500
        </div> <br>
      <q-btn color="teal-11" >
        Booked
        </q-btn>
      </div>
    </div>

     </div>
      </div>
      <div class="col">
      <div class="q-pa-md">
      <q-date
      v-model="date"
      today-btn
    />
    </div>
      </div>
    </div>
  </div>
</template>

<script>

import { defineComponent } from 'vue'
import { ref } from 'vue'
// import VueApexCharts from "vue3-apexcharts";
// const app = createApp(App);
// app.use(VueApexCharts);
export default defineComponent({
  name: 'IndexPage' ,
  // VueApexCharts app = new Vue({

//   el: '#appl',
//   data: function() {
//     return {
//       options: {
//         chart: {
//           id: 'vuechart-example'
//         },
//         xaxis: {
//           categories: [1991, 1992, 1993, 1994, 1995, 1996, 1997, 1998]
//         }
//       },
//       series: [{
//         name: 'series-1',
//         data: [30, 40, 45, 50, 49, 60, 70, 91]
//       }]
//     }
//   }
// });
setup () {
    return {
      date: ref('2019/02/01')
    }
  }

})
</script>
<style lang="sass" scoped>
.row > div
  padding: 10px 15px
  background: rgba(247, 251, 252)
  border: 1px solid rgba(86,61,124,.2)
.row + .row
  margin-top: 1rem
</style>


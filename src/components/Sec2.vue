<template>
<v-container grid-list-md>

<v-flex xs12 xl8 ma-auto>
   <v-layout row wrap>
   <Scrollama @step-enter="stepEnterHandler" :offset="0.5">
   <div data-step="1">
   <v-flex xs12 pa-5 id="article-1" class="mnp" ref="art1" >
    <articleOne />
   </v-flex>
   </div>

  <div data-step="2">
   <v-flex xs12 pa-5 id="article-2" class="mnp" ref="art2">
    <articleTwo />
   </v-flex>
   </div>
  <div data-step="3">
   <v-flex xs12 pa-5 id="article-3"  class="mnp" ref="art3">
    <articleThree />
   </v-flex>
   </div>
      </Scrollama>
   </v-layout>

   </v-flex>

   </v-container>
</template>
<script>
import 'intersection-observer'
import Scrollama from 'vue-scrollama'
import articleOne from '@/components/articleOne'
import articleTwo from '@/components/articleTwo'
import articleThree from '@/components/articleThree'

  export default {
    data () {
      return {
        articles:[
            {title:'Cannabis as a medicne',
             text:'Medical cannabis,is cannabis and cannabinoids that are recommended by doctors for their patients. Evidence suggests that cannabis can reduce nausea and vomiting during chemotherapy, improve appetite in people with HIV/AIDS, and reduce chronic pain and muscle spasms.The Cannabis plant has a history of medicinal use dating back thousands of years in many cultures .Medical cannabis can be administered through a variety of methods, including capsules, lozenges, tinctures, dermal patches, oral or dermal sprays, cannabis edibles, and vaporizing or smoking dried buds.',
             img:'/home-1.jpg',
             aurtor:'Din Ashkenazi',
             Date:'24 Oct',
             }
        ],
      }
    },
    components:{
        articleOne, articleThree , articleTwo,  Scrollama
    },
    methods: {
    stepEnterHandler ({element, index, direction}) {
    const x = index;
    const { art1 } = this.$refs
     const { art2 } = this.$refs
    const { art3 } = this.$refs
    const timeline = new TimelineLite() 
    switch(x){
      case 0:
        timeline.to(art1, 2, { 
                y:-10,
                ease: Power2.easeOut,
                opacity:1,
        });
        break;
        case 1:

         timeline.to(art2, 2, { 
                y:-10,
                ease: Power2.easeOut,
                opacity:1,
        });
        break;
        case 2:
    
         timeline.to(art3, 2, { 
                y:-10,
                ease: Power2.easeOut,
                opacity:1,
        });
        break;
    }
    
      } 
  },
  }
</script>
<style scoped>
.article-img{
width:350px;
height:250px;
}
.display-1{
  text-decoration: underline;
}
.article-title{
    color:#707070;
}
#article-1{
  opacity:0;
}
#article-2{
  opacity:0;
}
#article-3{
  opacity:0;
}
</style>

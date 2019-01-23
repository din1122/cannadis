<template>
<v-container pa-5 grid-md-list class="mnp2">
<Scrollama @step-enter="stepEnterHandler" :offset="0.5">
<v-layout row wrap>


<v-flex xs12 xl7 class="left-section pa-5" ref="leftbox" data-step="1">
    <div class="pb-4"><span class="display-2 about-title"> About us </span></div>
    <p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem

Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem

</p>
</v-flex>



<v-flex xs12 xl3 offset-xs0 offset-xl2  data-step="2"  ref="rightbox" class="right-section m-pt-5">
    <v-card >
    <v-card-title class="white--text">About</v-card-title>
    <v-card-text class="fill-height">
    <v-layout align-center justify-space-between column fill-height>
    <v-flex>
        <v-layout row wrap>
            <v-flex xs4 >
                <div class="img-circle">
                    <img :src="require('@/assets/dinashkenazi.png')" alt="home-1-cannabis" class="Profile-img">
                </div>
            </v-flex>
            <v-flex xs8 pb-5 class="text-xs-left">
                        <span class="body-2 underline">Din Ashkenazi</span><br>
                        <span>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem
                        Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem
                    </span>
            </v-flex>
        </v-layout>
    </v-flex>
    <v-flex>
        <v-layout row wrap>
            <v-flex xs4 >
                <div  class="img-circle">
                    <img :src="require('@/assets/ran.png')" alt="home-1-cannabis" class="Profile-img">
                </div>
            </v-flex>
            <v-flex xs8 class="text-xs-left">
                        <span class="body-2 underline">Ran Aflalo</span><br>
                        <span>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem
                         Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem
                        Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem
                    </span>
            </v-flex>
        </v-layout>
     </v-flex>  
    </v-layout>
    </v-card-text>
    </v-card>
</v-flex>


</v-layout>
</Scrollama>
</v-container>
</template>

<script>
import 'intersection-observer'
import Scrollama from 'vue-scrollama'
export default {
  data() {
    return {
  
    }
  },
  components:{
      Scrollama
  },
  methods: {
    stepEnterHandler ({element, index, direction}) {
        const timeline = new TimelineLite() 
        const { leftbox } = this.$refs;
        const { rightbox } = this.$refs;
        const x = index;
        console.log(x)
        switch(x){
            case 0:
               timeline.to(leftbox, 2, { 
               
                ease: Power2.easeOut,
                opacity:1,
                });
                timeline.to(rightbox, 2, { 
                ease: Power2.easeNone,
                opacity:1,
                delay:-1.5
                });
                break;
             
         
               
        }
    }
  },
}
</script>


<style scoped>

.v-card__title{
background: #78b821;
}
.Profile-img{
   border-radius:50%;
     width: 90px;
    height: 90px;
    object-fit:cover;
}
.left-section{
    background:white;
      background:white;
    -webkit-box-shadow: 0px 2px 1px -1px rgba(0,0,0,0.2), 0px 1px 1px 0px rgba(0,0,0,0.14), 0px 1px 3px 0px rgba(0,0,0,0.12);
      box-shadow: 5px 7px 13px -1px rgba(0,0,0,0.2), 0px 1px 1px 0px rgba(0,0,0,0.14), 0px 1px 3px 0px rgba(0,0,0,0.12);
      opacity:0;
}
.right-section{
    opacity:0
}
.about-title{
    border-left: 3px solid #78B821;
    padding-left: 15px;

}

</style>
<template>
<div>
<Scrollama @step-enter="stepEnterHandler" :offset="0.5" >
<v-container pa-5 grid-xs-list  class="container main mnp" >
<v-layout row wrap fill-height class="h-auto">
            <v-layout column fill-height>
         
              <v-flex xs12 style="height:380px;" class="product-1 product-box" data-step="1" ref="prod1" >
             <div class="floating-div" slot="activator">
                    <div class="text">
                    <p class="mb-2 text--black underline display-1">Cannabis store</p><br>
                    <span class="text--black">There are various extraction methods</span>
                    </div>
               </div>
                 <img :src="require('@/assets/prod-1.jpg')" alt="home-1-cannabis" class="product-img"  @click="dialog1 = true">
              </v-flex>
       
          
            <v-flex xs12 style="height:380px;" class="product-2 product-box" data-step="2" ref="prod2" >
             <div class="floating-div"  >
                     <div class="text">
                    <p class="mb-2 text--black underline display-1">Cannabis store</p><br>
                    <span class="text--black">There are various extraction methods</span>
                    </div>
               </div>
                 <img :src="require('@/assets/prod-3.jpg')" alt="home-1-cannabis" class="product-img" @click="dialog2 = true">
              </v-flex>
       
            </v-layout>
    
           <v-flex d-flex xs12 sm6 md4 fill-height data-step="3" class="product-3 h-auto" ref="prod3" >
                <div class="product-box">
                 <div class="floating-div">
                      <div class="text">
                    <p class="mb-2 text--black underline display-1">Cannabis store</p><br>
                    <span class="text--black">There are various extraction methods</span>
                    </div>
               </div>
                <img :src="require('@/assets/prod-2.png')" alt="home-1-cannabis" class="product-img" @click="dialog3 = true">
                </div>
            </v-flex>
     
      
</v-layout>

</v-container>

    <v-dialog v-model="dialog1" width="1400px" >
    <v-card class="main">

    <v-card-title class="card-title">
    <v-spacer></v-spacer>
    <v-icon @click="dialog1 = false" small >close</v-icon>
    </v-card-title>
      <v-card-text>
        <v-layout row wrap>
        <v-flex xs4>
        <div class="img-box">
         <img :src="require('@/assets/prod-1.jpg')" alt="home-1-cannabis" class="dialog-img elevation-4">
         </div>
        </v-flex>
        <v-flex xs8>
        <p>
        	<p>
								Currently, the two main cannabinoids from the marijuana plant that are of medical interest are THC and
								CBD.&nbsp;
							</p>

							<p>
								THC can increase appetite and reduce nausea. THC may also decrease pain, inflammation (swelling and redness),
								and muscle control problems.Unlike THC, CBD is a cannabinoid that doesn&#39;t make people &quot;high.&quot;
								These drugs aren&#39;t popular for recreational use because they aren&#39;t intoxicating. It may be useful in
								reducing pain and inflammation, controlling epileptic seizures, and possibly even treating mental illness and
								addictions. Many researchers, including those funded by the National Institutes of Health (NIH), are continuing
								to explore the possible uses of THC, CBD, and other cannabinoids for medical treatment.
							</p>



							<p>
								For instance, recent animal studies have shown that marijuana extracts may help kill certain cancer cells and
								reduce the size of others. Evidence from one cell culture study with rodents suggests that purified extracts
								from whole-plant marijuana can slow the growth of cancer cells from one of the most serious types of brain
								tumors. Research in mice showed that treatment with purified extracts of THC and CBD, when used with radiation,
								increased the cancer-killing effects of the radiation.<a href="#references"><sup>10</sup></a>

								<p>
        </p>
        </v-flex>
        <v-flex >
          <p class="display-2 dialog-title ">This is main title</p>
        </v-flex>
        <v-flex xs3>
          <v-btn large class="dialog-btn">Buy</v-btn>
        </v-flex>
        </v-layout>
      </v-card-text>
    </v-card> 
      </v-dialog>
    <v-dialog v-model="dialog2" width="1400px" >
    <v-card class="main">

    <v-card-title class="card-title">
    <v-spacer></v-spacer>
    <v-icon @click="dialog2 = false" small >close</v-icon>
    </v-card-title>
      <v-card-text>
        <v-layout row wrap>
        <v-flex xs4>
        <div class="img-box">
         <img :src="require('@/assets/prod-3.jpg')" alt="home-1-cannabis" class="dialog-img elevation-4">
         </div>
        </v-flex>
        <v-flex xs8>
        <p>
        	<p>
								Currently, the two main cannabinoids from the marijuana plant that are of medical interest are THC and
								CBD.&nbsp;
							</p>

							<p>
								THC can increase appetite and reduce nausea. THC may also decrease pain, inflammation (swelling and redness),
								and muscle control problems.Unlike THC, CBD is a cannabinoid that doesn&#39;t make people &quot;high.&quot;
								These drugs aren&#39;t popular for recreational use because they aren&#39;t intoxicating. It may be useful in
								reducing pain and inflammation, controlling epileptic seizures, and possibly even treating mental illness and
								addictions. Many researchers, including those funded by the National Institutes of Health (NIH), are continuing
								to explore the possible uses of THC, CBD, and other cannabinoids for medical treatment.
							</p>



							<p>
								For instance, recent animal studies have shown that marijuana extracts may help kill certain cancer cells and
								reduce the size of others. Evidence from one cell culture study with rodents suggests that purified extracts
								from whole-plant marijuana can slow the growth of cancer cells from one of the most serious types of brain
								tumors. Research in mice showed that treatment with purified extracts of THC and CBD, when used with radiation,
								increased the cancer-killing effects of the radiation.<a href="#references"><sup>10</sup></a>

								<p>
        </p>
        </v-flex>
        <v-flex >
          <p class="display-2 dialog-title ">This is main title</p>
        </v-flex>
        <v-flex xs3>
          <v-btn large class="dialog-btn">Buy</v-btn>
        </v-flex>
        </v-layout>
      </v-card-text>
    </v-card> 
      </v-dialog>
    <v-dialog v-model="dialog3" width="1400px" >
    <v-card class="main">

    <v-card-title class="card-title">
    <v-spacer></v-spacer>
    <v-icon @click="dialog3 = false" small >close</v-icon>
    </v-card-title>
      <v-card-text>
        <v-layout row wrap>
        <v-flex xs4>
        <div class="img-box">
         <img :src="require('@/assets/prod-2.png')" alt="home-1-cannabis" class="dialog-img elevation-4">
         </div>
        </v-flex>
        <v-flex xs8>
        <p>
        	<p>
								Currently, the two main cannabinoids from the marijuana plant that are of medical interest are THC and
								CBD.&nbsp;
							</p>

							<p>
								THC can increase appetite and reduce nausea. THC may also decrease pain, inflammation (swelling and redness),
								and muscle control problems.Unlike THC, CBD is a cannabinoid that doesn&#39;t make people &quot;high.&quot;
								These drugs aren&#39;t popular for recreational use because they aren&#39;t intoxicating. It may be useful in
								reducing pain and inflammation, controlling epileptic seizures, and possibly even treating mental illness and
								addictions. Many researchers, including those funded by the National Institutes of Health (NIH), are continuing
								to explore the possible uses of THC, CBD, and other cannabinoids for medical treatment.
							</p>



							<p>
								For instance, recent animal studies have shown that marijuana extracts may help kill certain cancer cells and
								reduce the size of others. Evidence from one cell culture study with rodents suggests that purified extracts
								from whole-plant marijuana can slow the growth of cancer cells from one of the most serious types of brain
								tumors. Research in mice showed that treatment with purified extracts of THC and CBD, when used with radiation,
								increased the cancer-killing effects of the radiation.<a href="#references"><sup>10</sup></a>

								<p>
        </p>
        </v-flex>
        <v-flex >
          <p class="display-2 dialog-title ">This is main title</p>
        </v-flex>
        <v-flex xs3>
          <v-btn large class="dialog-btn">Buy</v-btn>
        </v-flex>
        </v-layout>
      </v-card-text>
    </v-card> 
      </v-dialog>
</Scrollama>
</div>
</template>

<script>
import 'intersection-observer'
import Scrollama from 'vue-scrollama'
export default {
  data(){
    return{
      dialog1: false,
      dialog2: false,
      dialog3: false
    }
  },
  components:{
Scrollama
  },
  methods:{
      stepEnterHandler ({element, index, direction}) {
          const { prod1 } = this.$refs
          const { prod2 } = this.$refs
          const { prod3 } = this.$refs
             const timeline = new TimelineLite() 
          timeline.to(prod1, 1, { 
          x:0,
          ease: Power2.easeOut,
          opacity:1,
          }); 
            timeline.to(prod2, 0.5, { 
          y:0,
          ease: Power2.easeOut,
          opacity:1,
          }); 
            timeline.to(prod3, 0.5, { 
               x:0,
          ease: Power2.easeOut,
          opacity:1,
          }); 
    
  }

}
}
</script>
<style scoped>
.dialog-btn{
  background:var(--green) !important;
      color: white;
    width: 239px;
}
>>>.v-card__title {
  border-bottom:3px var(--green) solid;
  background:#e5e5e5;
}
.dialog-title{
  border-left:var(--green) solid 5px;
  margin-top:1%;
  padding-left:10px;
}

	.img-box {
		overflow: hidden;
		transition: all 0.2s ease-out;
    padding-right:40px;
	}


.left-d{
  border-right:4px solid black
}
.right-d{

}
.Profile-img{
   border-radius:50%;
     width: 90px;
    height: 90px;
}
.left-section{
    background:white;
    border:solid 2px rgb(211, 211, 211);
}
.about-title{
    border-left: 3px solid #78B821;
    padding-left: 15px;

}

.container{
height:800px;

}
.product-1{
   opacity:0;
   transform: matrix(1, 0, 0, 1, -251, 0);
}
.product-2{
    max-height: 40%;
    opacity:0;
     transform: matrix(1, 0, 0, 1, 0, 80);
}
.product-3{
    transform: matrix(1, 0, 0, 1, 251, 0);
    opacity:0
}
.product-img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    overflow: hidden;
    transition: all 0.2s ease;
    opacity:1;
}
.dialog-img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    overflow: hidden;
    transition: all 0.2s ease;
    opacity:1;
}
.product-box:hover .product-img {
  opacity: 0.3;
}

.product-box:hover .floating-div {
  opacity: 1;
}
.product-box{
    overflow: hidden;
    transition: all 0.2s ease-out;
    position: relative;
}


.product-img:hover{
  -webkit-transform:scale(1.05);
-ms-transform:scale(1.05);
transform:scale(1.05);
transition: all 0.2s ease;
 cursor:pointer;
 background:rgba(10, 0 0, 0.2);
}
.text {
  border:solid 2px #A19C72;
  width:350px;
  height:200px;
  color: black;
  font-size: 16px;
  padding: 16px 32px;
}
.floating-div {
  transition: .5s ease;
  opacity: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  text-align: center;
}
</style>
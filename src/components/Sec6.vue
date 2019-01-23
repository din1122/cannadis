<template>
<v-container pa-5 grid-list-xs class="mnp">
<v-layout row wrap class="mnp2">

<v-flex xs12 xl7 class="left-section pa-2">
<div class="border-left fill-height pa-5 mnp2">
<GmapTest />
    <div class="pb-4 pt-4"><span class="display-2 about-title "> Loaction </span></div>
    <p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem

Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem

</p>
</div>
</v-flex>

<v-flex xl3 xs12 offset-xl2 offset-xs0 class="m-pt-5 ">
<v-flex xs12>
        <v-card  >
        <v-card-title class="card-title"></v-card-title>
        <v-card-text class="pr-5 pl-5 fill-height">
        <v-layout column pa-2 fill-height>
            <v-flex text-xs-center pb-4>
            <span class="display-2 ">Contact Us</span>
            </v-flex>
            <v-flex>
            <span>Name:</span>
            <v-text-field outline>
            </v-text-field>
            </v-flex>
            <v-flex>
            <span>Email:</span>
            <v-text-field outline >
            </v-text-field>
            </v-flex>
            <v-btn large class="send-btn">Send</v-btn>

            <v-flex text-xs-center pt-5>
           
            
             <img class="logo" :src="require('@/assets/logo.png')">
             <p class="email-text">Info@Cannadis.com</p>
            <p class="phone-text"><span >Phone:</span><span> +972545468875 </span></p>
            </v-flex>
        </v-layout>
        </v-card-text>
        </v-card>
    </v-flex>
</v-flex>
</v-layout>
</v-container>
</template>
<script>
import GmapTest from '@/components/Gmap'
export default {
    components:{
        GmapTest
    }
}
</script>
<style scoped>
.phone-text{
    color:#a4a4a4;
}
.email-text{
    
    color:#747474;
}

.border-left{
 border:solid 2px #78b82196;
 padding:5px;
}
.logo{
    height:120px;
}
.send-btn{
    background:rgb(120, 184, 33) !important;
    color:white;
}
.Profile-img{
   border-radius:50%;
     width: 90px;
    height: 90px;
}
.left-section{
    background:white;
    -webkit-box-shadow: 0px 2px 1px -1px rgba(0,0,0,0.2), 0px 1px 1px 0px rgba(0,0,0,0.14), 0px 1px 3px 0px rgba(0,0,0,0.12);
      box-shadow: 5px 7px 13px -1px rgba(0,0,0,0.2), 0px 1px 1px 0px rgba(0,0,0,0.14), 0px 1px 3px 0px rgba(0,0,0,0.12);
}
.about-title{
    border-left: 3px solid #78B821;
    padding-left: 15px;

}
.card-title{
    background:#78B821;
    height: 8px;
    padding: 0px;
}
>>>.theme--light  .v-input__slot:hover {
    border: 2px solid rgb(120, 184, 33);
}
</style>
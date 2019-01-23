<template>
<div>
<section id="one">
   <sectionOne />
</section>

    <sectionTwo id="Two"/>

<section id="Three">
   <sectionThree />
</section>
<section id="Four">
   <sectionFour />
</section>
<section id="Five">
   <sectionFive />
</section>
<section id="Six">
   <sectionSix />
</section>
</div>
</template>
<script>
import sectionOne from '@/components/Home-sec1'
import sectionTwo from '@/components/Sec2'
import sectionThree from '@/components/Sec3'
import sectionFour from '@/components/Sec4'
import sectionFive from '@/components/Sec5'
import sectionSix from '@/components/Sec6'
export default{
   data(){
      return{

      }
   },
   components: {
    sectionOne, sectionTwo, sectionThree,sectionFour, sectionFive, sectionSix
  }
}
</script>

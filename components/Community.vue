<template>
  <!--Article section-->
  <section>
  <h2>VeBuWa in the Community</h2>
    <div class="community">
  <!--Image Area-->
        <img class="picnic" :src="require('/static/assets/images/picnic-cute.png')"/>
        <p class="comm-text">We are proud to be active in the Calgary Community either donating money or time to those in need. We take special interest in charities and outreach programs that aid those with disabilities who may be struggling more. Things like drop in centers and care facilities are high on our list of causes we support. We also actively host meet ups for food trucks in accessible community areas that anyone can attend.
  If you are a business or an individual looking to volunteer please feel free to contact us through twitter or through our contact page listing. Join us for our next meet up and share some love with our partners below.
        </p>
    </div>
  
  <!--LOGOS OF FICTIONAL CHARITIES-->

    <div class="charity">
        <img class="charities" :src="require('/static/assets/logos/blindful.png')"/>
        <img class="charities" :src="require('/static/assets/logos/elderly.png')"/>
        <img class="charities" :src="require('/static/assets/logos/obesity-center.png')"/>
    </div>
 <!--Twitter API-->

 <span>
   <a class="twitter-timeline" data-width="500" data-height="600" href="https://twitter.com/Vebuwa_Group?ref_src=twsrc%5Etfw">Tweets by Vebuwa_Group</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script> 
 </span>
    
</section>    
    
 
 
</template>
<!-- JS -->
<script>
export default {

}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Kosugi+Maru&display=swap');

.community { 
  display: flex;
  flex-wrap: wrap;
  text-align: center;
  align-items: center;
  align-content: center;
  flex-direction: column;
}
.picnic{
    max-width: 120ch;
}
.charity{
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  text-align: center;
  align-items: center;
  align-content: center;
  margin: 20px;
  justify-content: space-evenly;
  gap: 0px 50px;
}

.charities {
    display: flex;
    width: 150px;
  
}

h2 {
    font-family: 'Kosugi Maru', sans-serif;
    font-size: 4em;
    text-align: center;
    
}

section {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  text-align: center;
  align-items: center;
  align-content: center;
}
.comm-text{
    border: solid;
    border-color:#0bffb1;
    padding: 2em;
    max-width: 90ch;
}

</style>
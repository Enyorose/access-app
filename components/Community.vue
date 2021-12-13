<template>
  <!--Article section-->
  <section>
  <h2>VeBuWa in the Community</h2>
    <div class="community">
  <!--Image Area-->
        <img :src="require('/static/assets/images/picnic-cute.png')"/>
        <p>We are proud to be active in the Calgary Community either donating money or time to those in need. We take special interest in charities and outreach programs that aid those with disabilities who may be struggling more. Things like drop in centers and care facilities are high on our list of causes we support. We also actively host meet ups for food trucks in accessible community areas that anyone can attend.
  If you are a business or an individual looking to volunteer please feel free to contact us through twitter or through our contact page listing. Join us for our next meet up and some love with our partners below.
        </p>
    </div>
  
  <!--LOGOS OF FICTIONAL CHARITIES-->

    <div class="charity">
        <img class="charities" :src="require('/static/assets/logos/blindful.png')"/>
        <img class="charities" :src="require('/static/assets/logos/elderly.png')"/>
        <img class="charities" :src="require('/static/assets/logos/obesity-center.png')"/>
    </div>
 <!--Twitter API-->
    
</section>    
    
 
 
</template>
<!-- JS -->
<script>
export default {

}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Fuzzy+Bubbles:wght@700&display=swap');

.community { 
  display: flex;
  flex-wrap: wrap;
  text-align: center;
  align-items: center;
  align-content: center;
  max-width: 90ch;
}
.charity{
    display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  text-align: center;
  align-items: center;
  align-content: center;
  margin: 20px;
}

.charities {
    width: 150px;
}

h2 {
    font-family: 'Fuzzy Bubbles', cursive;
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


</style>
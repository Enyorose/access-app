<template>
  <!--Article section-->
  <section>
  <h2>VeBuWa in the Community</h2>
  <div class="community">
  <!--Image Area-->
  <img :src="require('/static/assets/images/picnic-cute.png')"/>
  <p>We are proud to be active in the Calgary Community either donating money or time to those in need. We take special interest in charities and outreach programs that aid those with disabilities who may be struggling more. Things like drop in centers and care facilities are high on our list of causes we support. We also actively host meet ups for food trucks in accessible community areas that anyone can attend.
  If you are a business or an individual looking to volunteer please feel free to contact us through twitter or through our contact page listing. Join for out next meet up and visit our partners below.
  </p>
  </div>
  </section>
  <!--LOGOS OF FICTIONAL CHARITIES-->
  <!--Twitter API-->
 
</template>
<!-- JS -->
<script>
export default {

}
</script>

<style lang="scss">

.community { 
  display: flex;
  flex-wrap: wrap;
  text-align: center;
  align-items: center;
  align-content: center;
  max-width: 90ch;
}
h2 {
  font-size: 5em;
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
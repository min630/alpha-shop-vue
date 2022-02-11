<template>
  <div class="home">
    <Navbar />
    <main>
      <div class="container">
        <h2 class="checkout-title">結帳</h2>
      </div>
      
      <div class="container">
        
        <!-- checkout stepper (Left)-->
        <div class="checkout-wrapper">

          <!-- step controller -->
          <StepController />
          
          <!-- form panel -->
          <div class="form-panel">
            <!-- <form id="a-form"> -->
            <AddressFrom />
            <DeliveryForm />
            <PaymentForm />
            <!-- </form> -->
          </div>
          
          <!-- Step control button -->
          <div class="btn-control d-flex justify-content-between">
            <button class="btn btn-outline d-none">&larr; 上一步</button>  <!-- 綁previousStep-->
            <button class="btn btn-primary">下一步 &rarr;</button>   <!-- 綁nextStep-->
            <!-- <button type="submit" class="btn btn-primary">確認下單</button>  要綁v-if最後一步，handleSubmit -->
          </div>
        </div>

        <!-- shopping Cart (Right)-->
        <ShoppingCart />
        
      </div>
    </main>
    <Footer />
  </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
import Footer from "../components/footer.vue";
import StepController from "../components/StepController.vue";
import AddressFrom from "../components/AddressForm.vue"
import DeliveryForm from "../components/DeliveryForm.vue"
import PaymentForm from "../components/PaymentForm.vue"
import ShoppingCart from "../components/ShoppingCart.vue"

export default {
  name: "Home",
  components: {
    Navbar,
    Footer,
    StepController,
    AddressFrom,
    DeliveryForm,
    PaymentForm,
    ShoppingCart,
  },
  data() {
    return {
      steps: 0,
      addressInfo: {
        gender: '',
        name: '',
        tel: '',
        email: '',
        city: '',
        address: '',
      },
      delivery: {
        deliveryMethods: '',
        deliveryFee: 0,
      },
      paymentInfo: {
        cardOwner: '',
        cardNumber: '',
        expirationDate: '',
        validationCode: '',
      }
    }
  },

};
</script>

<style lang="scss">
@import "../assets/scss/main.scss";
</style>
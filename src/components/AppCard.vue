<template>
  <div class="card">
    <div class="card--image">
      <IconSupport />
    </div>
    <div class="card--content flow">
      <h2>Order Summary</h2>
      <p>You can now support us</p>
      <div class="neutral">
        <div class="round">
          <iconCommunity />
        </div>
        <div>
          <p>Donation</p>
          <p>Starts as low 1$</p>
        </div>
        <button class="donate">Donate</button>
      </div>
      <div class="check-out">
        <button class="payment">Proceed to Payment</button>
        <button class="cancel">Cancel Order</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  /* background: linear-gradient(to right, #424, #398); */
  background: linear-gradient(to right, white, grey);
  margin: 0 auto;
  max-width: 450px;
  max-height: 800px;
  height: 100vh;
  text-align: center;
  border: 1px solid purple;
  border-radius: 20px;
  color: white;
  transition: transform 0.3s ease-in-out;
}

.card:hover {
  box-shadow: 2px 2px 2px 2px grey;
  transform: scale(1.1);
}

.card--image {
  padding: 12px;
  height: 150px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  border-radius: 20px;
}

.neutral {
  padding: 20px;
  text-align: center;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  background: rgba(128, 128, 128, 0.1);
}

.round {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  border-radius: 40px;
  height: 40px;
  width: 40px;
  cursor: pointer;
  background: rgba(128, 128, 128, 0.1);
  transition: transform 0.3s ease-out;
}

.round:hover {
  transform: scale(1.1);
}

/* .round svg path {
  cursor: pointer;
  border-radius: 20px;
} */

.donate {
  cursor: pointer;
  color: purple;
  background: inherit;
  border: none;
  text-decoration: underline purple;
  transition: transform 0.2s ease-in;
}

.donate:hover {
  transform: scale(1.1);
}

.flow > :where(:not(:last-child)) {
  margin-bottom: 1em;
}
.check-out {
  display: grid;
  gap: 1em;
  margin: 5px;
}
.payment {
  /* width: 448px; */
  background: purple;
  height: 40px;
  outline: none;
  border: none;
  color: white;
  border-radius: 20px;
  cursor: pointer;
  transition: transform 0.1s ease-in;
}

.payment:hover {
  transform: scale(1.1);
  box-shadow: 2px 2px 1px 1px linear-gradient(to right, #424, #398);
}

.cancel {
  /* width: 448px; */
  height: 40px;
  background: white;
  outline: none;
  border: none;
  color: grey;
  border-radius: 20px;
  cursor: pointer;
  transition: transform 0.2s linear;
}

.cancel:hover {
  transform: scale(1.1);
}
</style>

<script setup>
import IconCommunity from '@/components/icons/IconCommunity.vue'
import IconSupport from '@/components/icons/IconSupport.vue'
</script>

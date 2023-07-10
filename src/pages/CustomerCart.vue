<template>
  <q-page class="q-pa-md">
    <div class="text-h6 text-weight-bold q-mb-sm">Ball's Purchase History</div>

    <q-card class="shadow-16 q-mb-sm" style="border-radius: 8px" flat bordered>
      <q-card-section horizontal>
        <q-img
          class="col-2"
          width="120px"
          :ratio="1 / 1"
          src="https://cdn.quasar.dev/img/avatar.png"
        />

        <q-card-section>
          <q-card-section class="flex column items-evenly" style="width: 100%">
            <div class="text-h5 text-weight-bold">Sex</div>

            <div class="text-h6 text-bold">
              {{
                price * quantity > 0
                  ? `${price} * ${quantity} = ${price * quantity}`
                  : ''
              }}
              {{
                price * quantity === 0
                  ? 'Free'
                  : price * quantity === 1
                  ? 'Re.'
                  : 'Rs.'
              }}
            </div>
          </q-card-section>
        </q-card-section>
      </q-card-section>
    </q-card>
    <div class="text-h6 text-weight-bold q-mt-sm">Total Amount: sex rs.</div>
  </q-page>
</template>

<script setup lang="ts">
let price = 69;
let quantity = 2;
</script>

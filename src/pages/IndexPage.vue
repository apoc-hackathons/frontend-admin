<template>
  <q-page class="" padding>
    <div class="text-h6 text-weight-bold q-mb-sm">Current Customers</div>

    <q-card class="" style="border-radius: 8px">
      <q-list>
        <q-item clickable v-ripple to="/customerdata">
          <q-item-section avatar>
            <q-avatar>
              <img src="https://cdn.quasar.dev/img/avatar.png" />
            </q-avatar>
          </q-item-section>
          <q-item-section>John Doe</q-item-section>
        </q-item>
      </q-list>
    </q-card>
  </q-page>
</template>

<script setup lang="ts"></script>

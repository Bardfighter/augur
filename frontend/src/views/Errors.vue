<!-- #SPDX-License-Identifier: MIT -->
<template>
  <d-container fluid class="main-content-container px-4 pb-4">
    <!-- Error -->
    <div class="error">
      <div class="error__content">
        <h2>500</h2>
        <h3>Something went wrong!</h3>
        <p>There was a problem on our end. Please try again later.</p>
        <!-- <v-btn to ="/Dashboard">Back</v-btn> -->
        <d-button pill @click="$router.go(-1)">&larr; Go Back</d-button>
        <a href="https://github.com/chaoss/augur/issues/new/choose ">Report Bug</a>
      </div>
    </div>
  </d-container>
</template>

<script lang="ts">
import { Vue } from 'vue-property-decorator';
export default class Errors extends Vue {}
</script>

<style scoped>
a{
  margin-top: 20px;
}
</style>
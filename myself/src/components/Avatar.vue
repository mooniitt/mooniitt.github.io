<script setup>
import Atropos from 'atropos';
import { onMounted } from 'vue';
// Initialize

onMounted(
  ()=>{
    const myAtropos = Atropos({
    el: '.my-atropos',
    // rest of parameters
    });
  }
)
// console.log(Atropos)
</script>

<template>
  <div class="atropos my-atropos">
  <!-- scale container (required) -->
  <div class="atropos-scale">
    <!-- rotate container (required) -->
    <div class="atropos-rotate">
      <!-- inner container (required) -->
      <div class="atropos-inner">
        <!-- put your custom content here -->
        <!-- <div>
          <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="250" height="250" />
        </div> -->
        
        <img
                src="https://atroposjs.com/images/header/atropos-bg.svg"
                data-atropos-offset="-4.5"
              />
              <img
                class="layer"
                src="https://atroposjs.com/images/header/atropos-mountains.svg"
                data-atropos-offset="-2.5"
              />
              <img
                class="layer"
                src="https://atroposjs.com/images/header/atropos-forest-back.svg"
                data-atropos-offset="0"
              />
              <img
                class="layer"
                src="https://atroposjs.com/images/header/atropos-forest-mid.svg"
                data-atropos-offset="2"
              />
              <img
                class="layer"
                src="https://atroposjs.com/images/header/atropos-forest-front.svg"
                data-atropos-offset="4"
              />
      </div>
    </div>
  </div>
</div>
</template>

<style scoped>
.my-atropos {
  width: 631px;
  position: relative;
}

.layer {
  position: absolute;
  top: -5%;
  left: -5%;
  width: 110%;
  height: 110%;
}

</style>
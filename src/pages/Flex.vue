<template>
  <q-page >
    <div class="row q-mb-md">
      <div class="col bg-primary">1</div>
      <div class="col bg-secondary">2</div>
      <div class="col bg-accent">3</div>
    </div>
    <div class="row q-mb-md justify-center"> <!-- 12 cols -->
      <div class="col col-4 bg-primary">1</div>
      <div class="col col-4 bg-secondary">2</div>
    </div>
    
    <div class="row q-mb-md justify-end"> <!-- 12 cols -->
      <div class="col col-4 bg-primary">1</div>
      <div class="col col-4 bg-secondary">2</div>
    </div>
    
    <div class="row q-mb-md justify-between"> <!-- 12 cols -->
      <div class="col col-4 bg-primary">1</div>
      <div class="col col-4 bg-secondary">2</div>
    </div>
    
    <q-separator spaced />
    
    <div class="row q-mb-md justify-between"> <!-- 12 cols -->
      <div class="col-12 col-sm-6 col-md-4 bg-primary">1</div>
      <div class="col-12 col-sm-6 col-md-4 bg-secondary">2</div>
    </div>
    
    <q-separator spaced/>
    
    <div class="row q-mb-md justify-between">
      <div class="square-box bg-primary"></div>
      <div class="square-box bg-secondary"></div>
      <div class="square-box bg-accent"></div>
    </div>
    
    <div class="row q-mb-md justify-end">
      <div class="square-box bg-primary"></div>
      <div class="square-box bg-secondary"></div>
      <div class="square-box bg-accent"></div>
    </div>
    
    <div class="row q-mb-md justify-around">
      <div class="square-box bg-primary"></div>
      <div class="square-box bg-secondary"></div>
      <div class="square-box bg-accent"></div>
    </div>
    
    <div class="column q-mb-md items-center bg-dark">
      <div class="square-box bg-primary"></div>
      <div class="square-box bg-secondary"></div>
      <div class="square-box bg-accent"></div>
    </div>
    
    <div class="column q-mb-md items-end bg-dark">
      <div class="square-box bg-primary"></div>
      <div class="square-box bg-secondary"></div>
      <div class="square-box bg-accent"></div>
    </div>
    
    <div class="column custom-height q-mb-md items-center justify-between bg-dark">
      <div class="square-box bg-primary"></div>
      <div class="square-box bg-secondary"></div>
      <div class="square-box bg-accent"></div>
    </div>
    <div class="column custom-height q-mb-md items-center justify-between bg-dark">
      <div class="square-box bg-primary"></div>
      <div class="square-box self-end bg-secondary"></div>
      <div class="square-box bg-accent"></div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Flex'
})
</script>

<style scoped>
.col, .col-4, .col-6 .col-12{
  height: 50px;
}

.square-box{
  height: 50px;
  width: 50px;
}

.custom-height{
  height: 300px;
}
</style>

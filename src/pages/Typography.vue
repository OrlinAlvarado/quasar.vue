<template>
  <q-page class="flex column q-pa-md">
    <span class="text-h1">Headline 1</span>
    <span class="text-h2">Headline 2</span>
    <span class="text-h3">Headline 3</span>
    <span class="text-h4">Headline 4</span>
    <span class="text-h5">Headline 5</span>
    <span class="text-h6">Headline 6</span>
    
    <q-separator />
    <span class="text-subtitle1">Subtitle 1</span>
    <span class="text-subtitle2">Subtitle 2</span>
    
    <q-separator />
    
    <p class="text-body1">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Minima molestiae nisi esse quas consectetur eos, doloremque voluptates alias pariatur nostrum incidunt libero, molestias, voluptatum quia illo cumque placeat sunt ipsum.</p>
    <p class="text-body2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae officiis, quisquam maxime impedit nesciunt quas delectus at, consequuntur natus dolores perferendis illum ea sapiente modi? Laborum, beatae. Suscipit, mollitia doloribus.</p>
    
    <span class="text-weight-thin">Nostrud veniam nostrud consequat adipisicing ullamco sit magna sunt veniam est nisi.</span>
    <span class="text-weight-light">Cupidatat sunt ullamco quis cillum proident laborum eu voluptate in ea veniam eu quis nostrud.</span>
    <span class="text-weight-regular">Occaecat eiusmod in do in tempor minim mollit.</span>
    <span class="text-weight-medium">Id occaecat duis tempor id dolore voluptate occaecat exercitation ullamco qui eu Lorem.</span>
    <span class="text-weight-bold">Sint non anim ad aliquip cillum labore.</span>
    <span class="text-weight-bolder">Tempor dolore veniam magna id consequat commodo nisi pariatur minim aute sint commodo ipsum officia.</span>
    
    <q-btn 
      color="primary"
      :label=" sideMenuOpen ? 'Cerrar menú lateral' : 'Abrir menú lateral'"
      class="q-mt-md"
      @click="toggleSideMenu"
    />
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';
import useUI from 'src/composables/useUI';

export default defineComponent({
  name: 'Typography',
  setup(){
    
    const { sideMenuOpen, toggleSideMenu } = useUI()
    return {
      toggleSideMenu,
      sideMenuOpen
    }
  }
})
</script>

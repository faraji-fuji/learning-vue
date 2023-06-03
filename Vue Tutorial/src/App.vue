<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import GettingStarted from './components/GettingStarted.vue'
import DeclarativeRendering from './components/DeclarativeRendering.vue'
import AttributeBindings from './components/AttributeBindings.vue'
import EventListeners from './components/EventListeners.vue'
import FormBindings from './components/FormBindings.vue'
import ConditionalRendering from './components/ConditionalRendering.vue'
import ListRendering from './components/ListRendering.vue'
import ComputedProperty from './components/ComputedProperty.vue'
import LifecycleAndTemplateRefs from './components/LifecycleAndTemplateRefs.vue'
import Watchers from './components/Watchers.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>
  </header>

  <main>
    <!-- <TheWelcome /> -->
    <GettingStarted />
    <DeclarativeRendering />
    <AttributeBindings />
    <EventListeners />
    <FormBindings />
    <ConditionalRendering />
    <ListRendering />
    <ComputedProperty />
    <LifecycleAndTemplateRefs />
    <Watchers />
  </main>

</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>

<template>
  <div id="app">
    <Index />
  </div>
</template>

<script>
import Index from "./components/index";


export default {
  name: "App",
  components: { Index },
};
</script>

<style>
@import url('https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/css/bootstrap.min.css');
@import url('https://cdn.jsdelivr.net/npm/jquery@3.6.0/dist/jquery.slim.min.js');
@import url('https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js');
@import url('https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/js/bootstrap.bundle.min.js');

@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900&display=swap');



#app{
  font-family: 'Montserrat';
}
</style>

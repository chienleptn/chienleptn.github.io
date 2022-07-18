<template>
  <b-col cols="12" lg="4">
        <b-card class="mb-2 title card">
          <b-card-title>
            <ion-icon :name=icon class="thin"></ion-icon>
            <h1>{{name}}</h1>
          </b-card-title>
          <b-card-text>
            <h4>{{subtitle}}</h4>
          </b-card-text>

          <div class="row center">
            <div v-for="button in buttons" v-bind:key="button.text" class="col-12">
              <Button :text="button.text" :dest="button.dest" />
            </div>
          </div>
        </b-card>
      </b-col>
</template>

<script>
import Button from "./Button.vue";
export default {
    components: {
        Button
    },
    props: ['name', 'subtitle', 'icon', 'buttons']
}
</script>

<style>

</style>
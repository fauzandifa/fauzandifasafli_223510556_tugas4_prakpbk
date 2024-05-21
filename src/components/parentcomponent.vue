<template>
  <div>
    <p>Data from Child: {{ childData }}</p>
    <child-component @dataSent="handleDataSent"></child-component>
    <slot></slot>
  </div>
</template>

<script>
import ChildComponent from './childcomponent.vue';

export default {
  name: 'ParentComponent',
  components: {
    ChildComponent
  },
  data() {
    return {
      childData: ''
    };
  },
  methods: {
    handleDataSent(data) {
      this.childData = data;
    }
  }
}
</script>

<style scoped>
div {
  background-color: #fff;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

p {
  font-size: 18px;
  color: #333;
  margin-bottom: 20px;
}
</style>

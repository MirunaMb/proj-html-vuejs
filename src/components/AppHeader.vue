<script>
// import MyComponent from "./components/MyComponent.vue";

export default {
  data() {
  return {
    dropDowns: [
      {
        items: [
          { text: 'Home', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      {
        items: [
          { text: 'Games', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      {
        items: [
          { text: 'Shop', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      {
        items: [
          { text: 'Pages', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      {
        items: [
          { text: 'Blog', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      {
        items: [
          { text: 'Contact', active: true },
          { text: 'Games Details', active: true },
          { text: 'Match Details', active: true },
        ]
      },
      
    ]
  };
},

};
</script>


<template>
  <div>
    <div v-for="(dropdown, index) in dropDowns" :key="index" class="dropdown">
      <button class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
        {{ dropdown.items[0].text }}
      </button>
      <ul class="dropdown-menu dropdown-menu-dark">
        <li v-for="(item, itemIndex) in dropdown.items" :key="itemIndex" :class="{ 'active': item.active }">
          <a class="dropdown-item" href="#" v-if="!item.divider">{{ item.text }}</a>
          <hr class="dropdown-divider" v-else-if="item.divider" />
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
<template>
    <div>
        <ul class="tabs text-xl font-normal flex space-between" style="color: #686F75">
            <li v-for="tab in tabs" :key="tab" class="tab">
                <a  class="tab-link cursor-pointer leading-8" 
                    :class="{ active: tab === selected }" 
                    @click="setTab(tab)"
                >{{ tab }}</a>
            </li>
        </ul>
        <slot></slot>
    </div>
</template>

<script>
export default {
  props: {
    tabs: {
      type: Array,
      required: true,
    },
    selected: {
      type: String,
      required: true,
    }
  },
  methods: {
    setTab(tab) {
      this.$emit('selected', tab);
    },
  },
};
</script>

<style scoped>
.tab {
    @apply mr-8;
}
.active {
    color: #171F28;
}
</style>
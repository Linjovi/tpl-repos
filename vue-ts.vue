<template>
  <div class="{{name}}">
    
  </div>
</template>

<script lang="ts">
import { Component, Vue, Prop } from 'vue-property-decorator'

@Component({
  name:"{{name}}"
})
export default class {% for item in name.split('-') %}{{item | capitalize}}{% endfor %} extends Vue {
  @Prop(type)private propName = propValue;
}
</script>
<style lang='scss' scoped >

</style>

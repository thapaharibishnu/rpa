<template>
  <div class="row">
       <div class="col  table-responsive pl-3 pr-3">
         <b-table striped class="" :items="items" :fields="fields"></b-table>
       </div>
  </div>
</template>

<script>
export default {
  props: ["data"],
  data() {
    return {
      items: this.data.rows,
      fields: this.data.fields
    };
  }
};
</script>

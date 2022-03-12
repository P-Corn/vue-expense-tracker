<template>
  <div>
    <h2 class="text-left mb-5">Monthly Budget</h2>
    <budget-table />
  </div>
</template>

<script>
import BudgetTable from '../components/BudgetTable.vue'

export default {
  name: 'Budget Options',
  components: {
    BudgetTable
  }
}
</script>
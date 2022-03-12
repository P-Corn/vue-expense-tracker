<template>
  <div>
    <transactions-data-table />
  </div>
</template>

<script>
import TransactionsDataTable from '../components/TransactionsDataTable.vue'

export default {
  name: 'RecentTransactions',
  components: {
    TransactionsDataTable
  }
}
</script>
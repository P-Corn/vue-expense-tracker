<template>
  <v-card>
    <v-simple-table>
      <template v-slot:default>
        <thead>
          <tr>
            <th class="text-left">
              Category
            </th>
            <th class="text-left">
              Amount
            </th>
          </tr>
        </thead>
        <tbody>
          <tr
            v-for="item in budgetData"
            :key="item"
            align="left"
          >
            <td>{{ item.categoryTitle }}</td>
            <td>{{ item.categoryAmount }}</td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>
  </v-card>
</template>

<script>
export default {
  name: 'BudgetTable',
  data: () => ({
    budgetData: [
      { categoryTitle: 'Food', categoryAmount: 20 },
      { categoryTitle: 'Gas', categoryAmount: 200 },
      { categoryTitle: 'Fun', categoryAmount: 400 },
      { categoryTitle: 'Car note', categoryAmount: 250 },
      { categoryTitle: 'Rent', categoryAmount: 500 },
    ]
  })
}
</script>
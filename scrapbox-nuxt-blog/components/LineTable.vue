<script setup>
const props = defineProps({ line: Object })
</script>

<template>
  <table class="table-fixed border-collapse">
    <thead>
      <tr>
        <th v-for="c in line.cells[0]" class="border border-gray-300 bg-gray-100 p-2">{{ c[0].text }}</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="cell in line.cells.filter((cell, index) => index > 0)">
        <td v-for="c in cell" class="border border-gray-300 p-2">{{ c[0].text }}</td>
      </tr>
    </tbody>
  </table>
</template>

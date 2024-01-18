<script setup>
//fetch the data from a server rout
const fetchEmployees = async () => {
  const (employees) = await sfetch("/api/employees");
};
const employees = fetchEmployees();
console.log(employees);
</script>

<template>
  <main>
    <h1>Employees</h1>
    <!-- render the fethced data-->>
    <pre>{{ employees }}</pre>
  </main>
</template>
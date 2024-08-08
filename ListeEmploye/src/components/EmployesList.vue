<template>
    <div class="employes-container">
      <h1>Liste des Employés</h1>
      <ol class="employes-list">
        <li v-for="employe in employes" :key="employe.id" class="employe-item">
          {{ employe.name }}
        </li>
      </ol>
    </div>
  </template>
  
  <script>
  export default {
    name: 'EmployesList',
    data() {
      return {
        employes: [
          { id: 1, name: 'Fatima Cisse' },
          { id: 2, name: 'Thillo Seme' },
          { id: 3, name: 'Omar Ndiaye' },
          { id: 4, name: 'Ousmane Ly' }
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .employes-container {
    max-width: 600px;
    margin: 0 auto;
    padding: 20px;
    text-align: center;
    background-color: #f9f9f9;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  
  .employes-list {
    list-style-type: decimal;
    padding-left: 20px;
  }
  
  .employe-item {
    padding: 10px;
    font-size: 18px;
    transition: background-color 0.3s ease;
  }
  
  .employe-item:hover {
    background-color: #e0e0e0;
  }
  </style>
  
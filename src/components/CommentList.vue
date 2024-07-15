<template>
    <div class="comment-list">
      <h3>Comentarios</h3>
      <ul>
        <!-- Aquí debes renderizar los comentarios -->
        <li>
          <!-- Aquí irá el texto del comentario -->
        </li>
      </ul>
    </div>
  </template>
  
  <script setup>
  // Recibir los comentarios como props
  const props = defineProps({
    comments: Array
  });
  </script>
  
  <style scoped>
  .comment-list {
    margin-top: 20px;
  }
  
  .comment-list ul {
    list-style-type: none;
    padding: 0;
  }
  
  .comment-list li {
    background: #f9f9f9;
    padding: 10px;
    margin-bottom: 10px;
    border-radius: 5px;
  }
  </style>
  
<template>
    <div class="blog-post">
      <!-- Selector de post -->
      <select>
        <!-- Opciones de posts -->
      </select>
      <div>
        <!-- Título del post -->
        <h2><!-- Aquí va el título del post --></h2>
        <!-- Contenido del post -->
        <p><!-- Aquí va el contenido del post --></p>
  
        <!-- Componente para mostrar los comentarios -->
        <CommentList />
  
        <!-- Componente para agregar un nuevo comentario -->
        <CommentForm />
      </div>
    </div>
  </template>
  
  <script setup>
  // Importar los componentes necesarios
  import { ref, onMounted, watch } from 'vue';
  import CommentList from './CommentList.vue';
  import CommentForm from './CommentForm.vue';
  
  // Datos de los posts (se obtendrán de un archivo JSON)
  const posts = ref([]);
  const selectedPostIndex = ref(0);
  
  // TODO: Cargar los datos de los posts desde el archivo JSON
  
  // Post seleccionado actualmente
  const selectedPost = ref(null);
  
  // TODO: Función para cargar el post seleccionado
  
  // Llamar a la función de carga al montar el componente
  onMounted(() => {
    // TODO: Llamar a la función para cargar los datos de los posts
  });
  
  // TODO: Función para agregar un comentario
  </script>
  
  <style scoped>
  .blog-post {
    text-align: left;
    margin: 20px auto;
    width: 50%;
    border: 1px solid #ccc;
    padding: 20px;
    border-radius: 10px;
  }
  
  select {
    margin-bottom: 20px;
    padding: 10px;
    font-size: 16px;
    width: 100%;
  }
  </style>
  
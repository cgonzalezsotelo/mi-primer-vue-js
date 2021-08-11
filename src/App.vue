<template>
  <div class="container">
        <h1 class="text-center p-5">Tabla de Usuarios</h1>
      <table class="table table-striped" id="table">
        <thead>
          <tr>
            <th scope="col">#</th>
            <th scope="col">Nombre</th>
            <th scope="col">Apellido</th>
            <th scope="col">RUN</th>
            <th scope="col">Fecha de nacimiento</th>
            <th scope="col">Edad</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(persona, index) in personas" :key="index">
            <th scope="row">{{persona.id}}</th>
            <td>{{persona.nombre}}</td>
            <td>{{persona.apellido}}</td>
            <td>{{persona.run}}</td>
            <td>{{persona.fechaNacimiento}}</td>
            <td>{{persona.edad}}</td>
          </tr>
        </tbody>
      </table>
    </div>
</template>

<script>
export default {
  name: 'App',
  data: () => ({
    personas: [{
      id: 1,
      nombre: "Esteban",
      apellido: "Méndez",
      run: "16.230.234-1",
      fechaNacimiento: "10-05-1986",
      edad: "35"
    },
    {
      id: 2,
      nombre: "Carla",
      apellido: "Soto",
      run: "17.783.983-9",
      fechaNacimiento: "25-02-1989",
      edad: "32"
    },
    {
      id: 3,
      nombre: "Camila",
      apellido: "Fuentes",
      run: "20.984.883-4",
      fechaNacimiento: "18-09-2000",
      edad: "21"
    }]
  })
}
</script>

<style>
</style>

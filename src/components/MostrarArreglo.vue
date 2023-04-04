<template>
    <table class="table table-hover">
        <thead class="bg-primary text-light">
            <th>Nombre</th>
            <th>Apellido</th>
            <th>Fecha nacimiento</th>
            <th>Edad</th>
        </thead>
        <tbody>
            <tr v-for="item in persona" :key="item">
                <td>{{item.nombre }}</td>
                <td>{{ item.Apellido}}</td>
                <td>{{ item.FechaNacimiento }}</td>
                <td>{{item.edad}}</td>
            </tr>
        </tbody>
    </table>
</template>

<script>
export  default {
 name: 'MostrarArreglo',
 data: function () {
    return { persona:[ {
        nombre: 'Miguel',
        Apellido: 'Rondanelli',
        FechaNacimiento: '18-11-88',
        edad: '34'
    },
    {
        nombre: 'Romina',
        Apellido: 'Ramirez',
        FechaNacimiento: '03-07-89',
        edad: '33'
    },
    {
        nombre: 'Fabrizio',
        Apellido: 'Rondanelli',
        FechaNacimiento: '02-08-90',
        edad: '32'
    }]
 }}
}
</script>



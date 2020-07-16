<template>
    <div>
        <h2>Cliente aqui</h2>
        <!-- :value="nome" data-binding, para exibir dados e não modificar -->
        <input type="text" :value="nome">
        <input type="text" :value="descricao">
       
        <!-- {{}} Interpolação -->
        <p>{{nome}}</p>
        <p>{{numero}}</p>
        <p>{{email}}</p>
        <p>{{idade}}</p>
        <p>{{descricao}}</p>
        <hr>
    </div>
</template>

<script>
export default {
    data(){
        return {
            nome: "Gabriel",
            numero: "96",
            email: "gabrielferreiralouredo@gmail.com",
            idade: "22",
            descricao: "Lore ipsum"
        }
    }

}
</script>

// Estilos ficam aqui
<style scoped>
    div{
        font-size: 16px;
    }

</style>
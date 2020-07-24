<template>
    <div id="cliente">
        <!-- <h4>Nome: {{nome}}</h4> -->
        <!-- <p>{{descricao}}</p> -->
        <!-- <p>Número: {{numero}}</p>
        <p>Email: {{email}}</p>
        <p>Idade: {{idade}}</p> -->


        <!-- :value="nome" data-binding, para exibir dados e não modificar -->
        <!--       
        <input type="text" :value="nome">
        <input type="text" :value="descricao"> -->

        <!-- v-model="" to-way-data-binding -> formularios, checkbox's -->
        <!-- <input type="text" v-model="nome"> -->
       
        <!-- {{}} Interpolação -->
        <!-- <p>{{nome}}</p>
        <p>{{numero}}</p>
        <p>{{email}}</p>
        <p>{{idade}}</p>
        <p>{{descricao}}</p>
        <hr> -->
    </div>
</template>

<script>
export default {
    data(){
        return {
            //nome: "Gabriel",
            numero: "96",
            email: "gabrielferreiralouredo@gmail.com",
            idade: "22",
            descricao: "Lore ipsum"
        }
    },
    props: {
        nome: String
    }

}
</script>

// Estilos ficam aqui
<style scoped>
    #cliente{
        background-color: #f4f4f5;
        padding: 1%;
        margin-bottom: 10px;

    }

</style>
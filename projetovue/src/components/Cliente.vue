<template>
    <div id="cliente">
        <!-- prop -->
        <!-- <p >{{nome}} {{idade}} {{email}}</p> -->
        <!-- prop do tipo objeto -->

        <!-- mesmo sendo falso o v-show não deleta o elemento -->
        <!-- <p v-show="showName == true">{{dados.nome}}</p> -->
        <p v-if="showName == true">{{dados.nome}}</p>
        <p v-else>Usuario escondeu o nome</p>
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
            // email: "gabrielferreiralouredo@gmail.com",
            // idade: "22",
            descricao: "Lore ipsum"
        }
    },
    props:{
        // nome: String,
        // idade: Number,
        // email: String,
        // prop do tipo objeto
        dados: Object,
        showName: Boolean
    }

}
</script>


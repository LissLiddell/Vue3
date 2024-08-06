<template>
    <div>
       <h3>{{ counter }}</h3>  <!--  aqui va el contador -->
       <!-- eventos: @ al inicio , este manda a llamar addCounter por evento @click-->
        <button @click="addCounter">Incrementar</button>
    </div>
</template>

<script>
// Option api
import { defineComponent } from 'vue';
//siempre se declara a mano el componente, es para tener mas control
export default defineComponent({
    //nombre componente
    name: 'CounterOption',
    //anexas componentes separados por comas que vayas a necesitar dentro de este componente
    components: {},
    // variables - elementos que se usan en el componente
    data() {
        let counter = 0
        // data retorna un objeto con todas las variables trabajadas
        return {counter}
        // retornarlo sin necesidad de definirlo
        // return {counter: 0}
    }, 
    //metodos del componente
    methods: {
        // en este ejemplo: funcion que se llama cada que se presiona el botón y aumentara el contador en 1
        //cada metodo se llama separado por , 
        addCounter(){
            this.counter++
        }
    }
})
</script>

<style scoped>
</style>
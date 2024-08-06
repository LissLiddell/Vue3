<template>
    <div>
        <h3>{{ counter }}</h3>
        <button @click="addCounter">Incrementar</button>
    </div>
</template>

<!-- funcion setup ya difine propiedadea y metodoa con metodo hooks cyclelife para engancharse a los momentos
 del ciclo de vida e ir actuando sobre el componente
 en Composition tienes mas control de la reactividad-->
<script>
import { defineComponent } from 'vue';
export default defineComponent({
    name: 'CounterComposition',
    setup(){
        let counter = 0
        const addCounter = () => {
            counter++
            console.log(counter)
        }
        return { counter, addCounter}
    }
})
</script>

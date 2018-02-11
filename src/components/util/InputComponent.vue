<template>
    <input 
        :type='tipo' 
        :placeholder="pl" 
        @input="get($event.target.value)"
        :required='requerido'/>
</template>

<script>
export default {
    name:'input-component',
    props:['tipo', 'pl', 'requerido'],
    methods: {
        get(valor){
            this.$emit('input', valor)
        }
    }
}
</script>

<style lang="less">
	@import "../../less/input";
</style>

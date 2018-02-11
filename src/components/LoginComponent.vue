<template>
    <div class="wrapper">
        <div class="container">
            <h1>{{ titulo }}</h1>
            
            <form class="form">
                <input-component 
                    :type="'text'" 
                    :placeholder="tituloUser" 
                    :required='requerido' 
                    v-model='form.user'>
                </input-component>

                <input-component 
                    :type="'password'" 
                    :placeholder="tituloPass" 
                    :required='requerido' 
                    v-model='form.pass'>
                </input-component>
                
                <button type="submit" id="login-button">Login</button>
            </form>
        </div>
        
        <ul class="bg-bubbles">
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
        </ul>
    </div>
</template>

<script>

import InputComponent from './util/InputComponent'

export default {
    name:'login-component',
    components:{
        InputComponent
    },
    data (){
        return {
            form:{
                user:'',
                pass:''
            },
            titulo: "Login",
            tituloUser: 'Usuario',
            tituloPass: 'Senha',
            requerido: false
        }
    }
}
</script>

<style lang="less">
    @import "../less/login";    
</style>

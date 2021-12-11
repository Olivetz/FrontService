<template>
    <Navbar :logOut="logOut"/>
    <div class="container mt-5">
        <h4>Bienvenido al inicio componente Home</h4>
        <Providers :ProvidersList="ProvidersList"/>
    </div>
    
    
   
</template>

<script>
import Navbar from './partials/Navbar.vue'
import Providers from './Providers.vue'

export default {
    name: 'Home',
    components: {
        Navbar,
        Providers
    },
    methods :{
        logOut(){
            this.$emit('logout');
        }
    },
    data() {
        return{
            ProvidersList:[{
                id: "61a9001467cd4c0e5b77aa12",
                name: "Limpieza profunda",
                tip_document: "tarjeta de identidad",
                num_document: 99091805,
                city: "Cali",
                address: "Calle 156 Av 34",
                phone_num: 789332,
                mobile_num: 30234879,
                social_security: 4321,
                value: 200000.0,
                password: "example",
                tip_user: "lavado"
            },
            {
                id: "61abceac82c27d1654471efa",
                name: "aseo profundo",
                tip_document: "cedula",
                num_document: 12233455,
                city: "Manizales",
                address: "calle 13 # 24-13",
                phone_num: 12230098,
                mobile_num: 3526342,
                social_security: 99999,
                value: 234565.0,
                password: "sisisisi",
                tip_user: "aseo"
            },
            {
                id: "61abcf0282c27d1654471efb",
                name: "aseo profundo",
                tip_document: "passport",
                num_document: 5555555,
                city: "bogota",
                address: "cerca de ahi",
                phone_num: 22222222,
                mobile_num: 3333333,
                social_security: 2222,
                value: 300000.0,
                password: "juanitoalimaña",
                tip_user: "perezoso"
            }, 
            {
                id: "61abcf0282c27d1654471efu",
                name: "aseo profundo",
                tip_document: "passport",
                num_document: 5555555,
                city: "bogota",
                address: "cerca de ahi",
                phone_num: 22222222,
                mobile_num: 3333333,
                social_security: 2222,
                value: 300000.0,
                password: "juanitoalimaña",
                tip_user: "perezoso"
            }]
        }
    }
}

</script>
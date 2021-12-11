<template>
    <h2>Lista de Proevedores</h2>
    <div class="container">
        <div class="card-deck">
            <div class="row">
                <div class="col-4" v-for="provider in ProvidersList" :key="provider.id">
                    <div class="card">
                        <img class="card-img-top" src="https://www.proveedores.com/site/category/productos-de-limpieza-industrial.jpg" alt="" height="250" width="200">
                        <div class="card-body">
                            <h5 class="card-title">{{provider.name}}</h5>
                            <p class="card-text">Es un proevedor</p>
                            <p class="card-text"><small class="text-muted">{{provider.tip_user}}</small></p>
                            <button class="btn btn-danger float-end"> Ver mas..</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
   name: 'Providers',
   props: ['ProvidersList']

}
</script>


<style>
    .card{
        margin-top:20px;
    }   
</style>

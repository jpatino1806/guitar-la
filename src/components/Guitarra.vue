<script setup>
const props = defineProps({
    guitarraProp: {
        type: Object,
        Required: true
    }
})

</script>


<template>
    <div class="col-md-6 col-lg-4 my-4 row align-items-center">
        <div class="col-4">
            <img class="img-fluid" :src="'/img/' + guitarraProp.imagen + '.jpg'"
                :alt="'imagen guitarra' + guitarraProp.nombre">
        </div>
        <div class="col-8">
            <h3 class="text-black fs-4 fw-bold text-uppercase">{{ guitarraProp.nombre }}</h3>
            <p>{{ guitarraProp.descripcion }}</p>
            <p class="fw-black text-primary fs-3">${{ guitarraProp.precio }}</p>
            <button type="button" class="btn btn-dark w-100 ">Agregar al Carrito</button>
        </div>
    </div><!-- FIN GUITARRA -->
</template>


<style lang="scss" scoped></style>
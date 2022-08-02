<template>
    <div class="entry-container mb-3 pointer p-2" @click="$router.push({ name: 'entry', params: { id: '10' } })">
        <!-- Titilo -->
        <div class="entry-title d-flex">
            <span class="text-success fs-5 fw-bold">12 de </span>
            <span class="mx-1 fs-5">Febrero</span>
            <span class="mx-2 fw-light">20022</span>
        </div>
        <div class="entry-description">
            asdasdasd
        </div>
    </div>
</template>

<script>
const months = ['Enero', 'Febrero', 'Marzo', 'Abril', 'Mayo', 'Junio', 'Julio', 'Agosto', 'Septiembre', 'Octubre', 'Noviembre', 'Diciembre']
const days = ['Domingo', 'Lunes', 'Martes', 'Miércoles', 'Jueves', 'Viernes', 'Sábado']


export default {
}
</script>

<style lang="scss" scoped>
.entry-container {
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;

    &:hover {
        background-color: lighten($color: grey, $amount: 45);
        transition: 0.2s all ease-in;
    }

    .entry-description {
        font-size: 12px;
    }
}
</style>
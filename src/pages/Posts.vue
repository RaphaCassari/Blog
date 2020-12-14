<template>
  <q-page padding>
    <!-- content -->
    <div class="row q-gutter-sm">
      <div class="col-sm-12 col-md-5" v-for="artigo in 10" :key="artigo">
        <q-card class="my-card">
      <q-img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7c/Cima_da_Conegliano%2C_God_the_Father.jpg/300px-Cima_da_Conegliano%2C_God_the_Father.jpg" style="width:200px"/>
        </q-card>
        <q-card
      class="my-card text-white"
      style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
    >
      <q-card-section>
        <div class="text-h6">Porrinha do texto</div>
        <div class="text-subtitle2">by Cassalindo</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ t1 }}
      </q-card-section>
    </q-card>
    <q-card-actions>
        <q-btn flat round icon="api" />
        <q-btn flat color="primary" >
          Botãozinho
        </q-btn>
        <q-btn push color="dark" label="Detalhes" class="full-width"/>
      </q-card-actions>
      </div>
    </div>

  </q-page>
</template>

<script>
export default {
  name: 'Posts',
  data () {
    return {
      t1: 'Raphael Lindo Maravilhoso'
    }
  }
}
</script>

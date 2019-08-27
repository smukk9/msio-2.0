<template>
  <div class="section">
    <div class="columns container is-centered">
      <div class="column is-11 is-offset-1">
        <h1 class="title has-text-centered">Archives</h1>
        <div class="section">
         <template>
    <section>

  <div class="container is-fluid">
  <div class="columns is-multiline">
    <div class="column is-one-quarter">
      <ArchiveCard></ArchiveCard>
    </div>
    <div class="column is-one-quarter">
      <ArchiveCard></ArchiveCard>
    </div>
    <div class="column is-one-quarter">
       <ArchiveCard></ArchiveCard>
    </div>
    <div class="column is-one-quarter">
       <ArchiveCard></ArchiveCard>
    </div>
    <div class="column is-one-quarter">
     <ArchiveCard></ArchiveCard>
    </div>
    <div class="column is-one-quarter">
       <ArchiveCard></ArchiveCard>
    </div>
    <div class="column is-one-quarter">
      <ArchiveCard></ArchiveCard> 
    </div>
  </div>
</div>

    </section>
</template>  
        </div>
      </div>
    </div>
  </div>
</template> 
<script>
import ArchiveCard from '~/components/UI/ArchiveCard.vue'
export default {
    components:{
        ArchiveCard
  },
  data() {
      return {
        
      }
  }
    }
</script>

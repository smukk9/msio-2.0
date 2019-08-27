<template>
            <b-collapse class="card" aria-id="contentIdForA11y3">
            <div
                slot="trigger" 
                slot-scope="props"
                class="card-header"
                role="button"
                aria-controls="contentIdForA11y3">
                <a href="/" class="card-header-title is-centered">
                    {{title}}
                    {{date}}
                </a>
                
                <a class="card-header-icon">
                    <b-icon
                        :icon="props.open ? 'menu-down' : 'menu-up'">
                    </b-icon>
                </a>
            </div>
            <div class="card-content">
                <div class="content">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.
                    <a>#buefy</a>.
                </div>
            </div>
            <footer v-if="isfooter" class="card-footer">
                <a class="card-footer-item">Save</a>
                <a class="card-footer-item">Edit</a>
                <a class="card-footer-item">Delete</a>
            </footer>
        </b-collapse>
</template>
<script>

export default {
       data () {
           return{
               isfooter:false,
               "title":"My first artile",
               "date":"12th August"
           }
     },
      
}
</script>
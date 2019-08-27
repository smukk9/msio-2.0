<template>
  <div class="section">
    <div class="columns container is-centered">
      <div class="column is-11 is-offset-1">
        <h1 class="title has-text-centered">Tags</h1>
        <div class="section">
          <template>
            <section>
              <Editor v-model="text" />
            </section>
          </template>
        </div>
      </div>
    </div>
  </div>
</template>  

<script>
import { Editor, Renderer, Toolbar } from 'vuetify-markdown-editor';

// CSS for Editor
import 'vuetify-markdown-editor/dist/vuetify-markdown-editor.css';

/* Editor is a Vue component
 * Renderer is the internal rendering function
 * Toolbar is a Vue component used for some WYSIWYG functions
 */

export default {
  components: {
    Editor
  },
  data() {
    return {
      text: ''
    };
  }
};
</script>
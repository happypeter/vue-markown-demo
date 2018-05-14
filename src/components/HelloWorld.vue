<template>
<div v-if="content">

<vue-markdown>
{{content}}

# hello
</vue-markdown>
</div>
</template>


<script>
import axios from 'axios'
import VueMarkdown from 'vue-markdown'
export default {
  name: 'HelloWorld',
  components: {
    VueMarkdown
  },
  data: () => ({
    content: ''
  }),
  created() {
    const uri =
      'https://raw.githubusercontent.com/happypeter/haoduoshipin/master/posts/videos/10.md'
    axios.get(uri).then(res => {
      this.content = res.data
      console.log('this.content', this.content)
    })
  }
}
</script>

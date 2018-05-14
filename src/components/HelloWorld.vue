<template>
<div>
  <vue-markdown> The # hhh time of **NOW** is : </vue-markdown>
  <vue-markdown> 

```js
console.log('hello')
```

  </vue-markdown>
    <vue-markdown>
### Solar System Exploration, 1950s – 1960s

- [ ] Mercury
- [x] Venus
- [x] Earth (Orbit/Moon)
- [x] Mars
- [ ] Jupiter
- [ ] Saturn
- [ ] Uranus
- [ ] Neptune
- [ ] Comet Haley
    </vue-markdown>
</div>
</template>


<script>
import VueMarkdown from 'vue-markdown'
export default {
  name: 'HelloWorld',
  components: {
    VueMarkdown
  }
}
</script>

---
pageClass: radio-page-class
---

# Radio
## 单选框组

<template>
  <div id="radio">
    <div class="radio-group">
        <co-radio-group :data="RadioData" v-model="val"></co-radio-group>
    </div>
  </div>
</template>

```html
<template>
  <div id="radio">
    <div class="radio-group">
        <co-radio-group :data="RadioData" v-model="val" @change="LogSomething"></co-radio-group>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
        RadioData: [{
          text: '选项1',
          value: '1'
        }, {
          text: '选项2',
          value: '2'
        }, {
          text: '选项3',
          value: '3'
        }],
        val: '1'
      }
  },
  methods: {
    LogSomething (val) {
      console.log(val)
    }
  }
}
</script>
```

<script>
export default {
  data () {
    return {
        RadioData: [{
          text: '选项1',
          value: '1'
        }, {
          text: '选项2',
          value: '2'
        }, {
          text: '选项3',
          value: '3'
        }],
        val: '1'
      }
  },
  methods: {
      LogSomething (val) {
      console.log(val)
    }
  }
}
</script>
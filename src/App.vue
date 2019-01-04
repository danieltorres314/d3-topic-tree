<template>
  <div id="app">
    <topic-tree :data="treeData"></topic-tree>
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body {
  margin: 0;
}
</style>
<script>
import TopicTree from './components/topic-tree'

export default {
  components: { TopicTree },
  data: () => ({
    treeData: {
      name: 'Science',
      link: null,
      hasChild: true,
      children: [
        {
          name: 'Physics',
          link: 'https://www.classmarker.com/online-test/start/?quiz=jet5c2ec48d2a97d',
          hasChild: true,
          children: [
            {
              name: 'Linear Motion 1',
              link: null,
              hasChild: true,
              children: [
                {
                  name: 'motion',
                  link: null,
                  hasChild: true,
                  children: [{ name: 'color1', link: null, hasChild: false }]
                },
                {
                  name: 'SUB-CATEGORY',
                  link: null,
                  hasChild: true,
                  children: [{ name: 'color', link: null, hasChild: false }]
                }]
            },
            { name: 'Linear motion 2', link: null, hasChild: false },
            { name: 'Linear motion 3', link: null, hasChild: false },
            { name: 'Linear motion 7', link: null, hasChild: false },
            { name: 'Linear motion 4', link: null, hasChild: false },
            { name: 'Linear motion 5', link: null, hasChild: false },
            { name: 'Linear motion 6', link: null, hasChild: false }
          ]
        },
        { name: 'Chemistry', link: null, hasChild: false },
        { name: 'Physical Science', link: null, hasChild: false },
        { name: 'Biology', link: null, hasChild: false },
        { name: 'Anatomy', link: null, hasChild: false },
        { name: 'Physiology', link: null, hasChild: false },
        { name: 'Zoology', link: null, hasChild: false },
        { name: 'Science', link: null, hasChild: false },
        { name: 'Physics - Intermediate', link: null, hasChild: false },
        { name: 'Biology', link: null, hasChild: false }
      ]
    }
  })
}
</script>

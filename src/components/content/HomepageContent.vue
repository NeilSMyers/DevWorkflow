<template>
  <div>
    <h1>DevWorkflow</h1>
    <p>{{ subtitle }}</p>
    <p>{{ marketingMessage }}</p>
  </div>
</template>

<script>


export default {
  name: "HomepageContent",
  data() {
    return {
     
    }
  },
  props: {
    subtitle: String,
    marketingMessage: String
  }
}
</script>

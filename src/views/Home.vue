<template>
  <div class="home">
    <HomepageContent :subtitle="subtitleContent" :marketingMessage="marketingMessage"/>
    <Auth formType="login" @update="handleLoginUpdate" />
    <Auth formType="register" @update="handleLoginUpdate" />
  </div>
</template>

<script>
import HomepageContent from "@/components/content/HomepageContent"
import Auth from "@/components/auth/Auth"

export default {
  name: 'home',
  data() {
    return {
      email: "",
      password: "",
      subtitleContent: "Manage your development projects",
      marketingMessage: "Sign up today to get started today"
    }
  },
  components: {
    HomepageContent,
    Auth
  },
  methods: {
    handleLoginUpdate(data) {
      console.log(data)
    }
  }
}
</script>

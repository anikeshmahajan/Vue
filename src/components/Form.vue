<template>
  <div>
       <div v-text="title"></div>
       <h2> {{testing}}</h2>

    <input v-model="name" type="text" name="" placeholder="Name Here" />
    <br /><br />
    <input v-model="email" type="email" name="email" placeholder="Email Here" />
    <br /><br />
    <input
      v-model="password"
      type="password"
      name="password"
      placeholder="Password Here"
    />
    <br /><br />
    <button @click="submit">Submit</button>
  </div>
</template>

<script>
export default {
  name: "Form",
  data() {
    return {
      name: "",
      email: "",
      password: "",
      title : "Welcome To The Form",
      testing :"TestDemo"
    };
  },
  methods: {
    submit() {
      alert("name is " + this.name + " email is " + this.email);
    },
  },
};
</script>
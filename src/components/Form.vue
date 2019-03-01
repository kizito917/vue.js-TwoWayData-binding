<template>
  <div>
    <h3 id="headerMsg">{{ headerMsg }}</h3>
    <form>
      <div id="form=header">
        <h3>Kindly Fill The Form Below</h3>
      </div>
      <div id="form-content">
        <label>Name:</label>
        <input type="text" v-model.lazy="form.name" placeholder="Enter Your Name"><hr>
        <label>Email:</label>
        <input type="email" v-model.lazy="form.email" placeholder="Enter Your Email"><hr>
        <label>Brief History About You:</label><br>
        <textarea v-model.lazy="form.history" ></textarea>
      </div><br>
      <div id="checkCenter">
        <label>Who are you?</label><br>
        <select v-model="form.who">
          <option v-for="skill in skills">{{ skill }}</option>
        </select>
      </div>
    </form>
    <div id="preview">
      <h3>{{ preview }}</h3>
      <p><strong>Name:</strong> {{ form.name }}</p>
      <p><strong>Email:</strong> {{ form.email }}</p>
      <p><strong>Brief History:</strong> </p>
      <p>{{ form.history }}</p>
    <p><strong>Category:</strong> {{ form.who }}</p>
    </div>
    <div id="form-footer">
        <p> {{ copyright }}</p>
      </div>
  </div>
</template>

<script>

export default {
  data () {
    return {
      headerMsg: "Vue.js Data Binding Input Form",
      form: {
        name: "",
        email: "",
        history: "",
        who: []
      },
      copyright: 'Designed By Brain.js',
      preview: 'My Form Preview',
      skills: ["Ninja", "Developer", "Hacker"]
    }
  }, 
  methods: {

  }
}
</script>

<style scoped>
#headerMsg{
  text-align: center;
    font-family: verdana;
    color: blue;
    word-spacing: 10px;
}
h3{
    text-align: center;
    font-family: verdana;
  }
hr{
    width: 350px;
  }
#form-footer{
  text-align: center;
  color: blue;
  word-spacing: 0.4em;
  letter-spacing: 0.2em;
}
#form-content{
  text-align: center;
  border: 2px solid;
  border-radius: 5px;
  border-color: dotted red;
}
#preview{
  text-align: center;
  border: 2px solid;
  border-radius: 5px;
  border-color: dotted red;
}
#checkCenter{
  text-align: center;
  border: 2px solid;
  border-radius: 5px;
  border-color: dotted red;
  margin-bottom: 20px;
}
textarea{
  margin-bottom: 20px;
}
strong{
  color: blue;
}
</style>

<template>

  <form  @submit.prevent="handleSubmit">  

    <h3>Sign Up</h3>
          
   <div class="form-group">
        <label>Email Address</label>
         <input type="email" class="form-control" v-model="email" placeholder="Email"/>
   </div>
    
   <div class="form-group">
        <label>Create Password</label>
         <input type="password" class="form-control" v-model="password" placeholder="Password"/>
   </div>
  

   <button class="btn btn-primary btn-block">Sign Up</button>


  </form>
    
</template>


<script>
import axios from 'axios'
export default {
    name: 'Register',
    data() {
        return {
                      
            email: '',
            password: ''
          
        }
        
    },
    
    methods: {
         handleSubmit() {
             const data = {
                 
                 email: this.email,
                 password: this.password
               
             };
             console.log(data);
             axios.post('http://localhost/8000/register' , data)
             .then(
                res => {
                     console.log(res)
                 }
             ).catch(
                 err => {
                     console.log(err)
                 }
             )
         }
   }
}
</script>
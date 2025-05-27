<template>
  <section>
     <h2>My Friends</h2>
   <ul>
    <friend-contact></friend-contact>
    <friend-contact></friend-contact>
   </ul>
  </section>
</template>

<script>
import FriendContact from './components/FriendContact.vue'
 export default  {
  components: { FriendContact },
    data(){
        return {
            friends:[
                {id:"manuel",name:"Manuel Lorenz",phone:"01234545",email:"yowyow@"},
                {id:"jack",name:"Jack Jones",phone:"555",email:"heyhey@"},
            ]
        }
    }
}
</script>
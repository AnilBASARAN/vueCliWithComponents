<template>
    <li>
        <h2>{{ friend.name }}</h2>
        <button @click="toggleDetails">{{ detailsAreVisible ? 'Hide' : 'Show' }}   Details</button>
        <ul v-if="detailsAreVisible" >
            <li><strong>Phone:</strong>{{ friend.phone }}</li>
            <li><strong>Email:</strong>{{ friend.email }}</li>
        </ul>
    </li>
</template>

<script>
export default {
    data(){
        return {
            detailsAreVisible:true,
            friend: {id:"jack",name:"Jack Jones",phone:"555",email:"heyhey@"}
        }
    },
    methods: {
        toggleDetails(){
            this.detailsAreVisible = !this.detailsAreVisible;
        }
    }
}

</script>
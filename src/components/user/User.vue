<template>
    <div>
        <h1>The Use Page</h1>
        <hr>
        <p>Loaded ID: {{id}}</p>
        <button @click="navigateToHome" class="btn btn-primary">Go to Home</button>
    </div>
</template>


<script>
    export default {
        methods: {
            navigateToHome(){
                this.$router.push({
                    path: '/'
                });
            }
        },
        data(){
            return {
                id: this.$route.params.id
            }
        }
        
    }
</script>
<template>
    <div>
        <h1>The Use Detail Page</h1>
        <p>User loaded has id: {{$route.params.id}}</p>
        <router-link 
            tag="button" 
            :to="link" 
            class="btn btn-primary">Edit User</router-link>
    </div>
</template>


<script>
    export default {
        data() {
            return {
                link: {
                    name: 'userEdit', 
                    params: {id: this.$route.params.id}, 
                    query: {locale: 'en', q:100},
                    hash: '#data'
                }
            }
        },
        beforeRouteEnter(to, from, next){
            //在外面不能获取this.link
            //这样获取：next(vm => {vm.link});
//            if(true){
//                next();
//            } else {
//                next(false);
//            }
        }
    }
</script>
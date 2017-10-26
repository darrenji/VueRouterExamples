<template>
    <div>
        <h1>The Use Detail Page</h1>
        <p>User loaded has id: {{$route.params.id}}</p>
        <router-link tag="button" :to="'/user/' + $route.params.id + '/edit'" class="btn btn-primary">Edit User</router-link>
    </div>
</template>
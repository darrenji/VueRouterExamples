<template>
    <div>
        <p>Please select a User</p>
        <hr>
        <ul class="list-group">
            <router-link tag="li" class="list-group-item" style="cursor:pointer" to="/user/1">User1</router-link>
            <router-link tag="li" class="list-group-item" style="cursor:pointer" to="/user/2">User2</router-link>
            <router-link tag="li" class="list-group-item" style="cursor:pointer" to="/user/3">User3</router-link>
        </ul>
    </div>
</template>
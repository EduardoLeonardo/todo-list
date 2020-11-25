<template>
    <div> 
        <form>
            <div class="form-group">
                <label for="exampleInputEmail1">Email address</label>
                <input type="email" class="form-control"  v-model="email" >
            </div>
            <div class="form-group">
                <label for="exampleInputPassword1">Password</label>
                <input type="password" class="form-control" v-model="password" id="exampleInputPassword1">
            </div>
            <button type="submit" class="btn btn-primary" v-on:click="show()">Submit</button>
        </form>
    </div>
</template>

<script>
export default {
    data() {
        return {
            email: "",
            password: ""          
        }
    
    },
    methods: {
        show: function () { console.log(this.email +'-' +this.password)}
    }

}
</script>

<style>

</style>
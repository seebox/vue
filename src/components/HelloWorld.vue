<style scoped>

</style>
<template>
<Layout>

</Layout>
    
</template>
<script>
    export default {
        data () {
            return {
                modal1: false
            }
        },
        methods: {
            ok () {
                this.$http.get('/user').then((response)=>{
                    alert(1);
                });
                
            },
            cancel () {
                this.$Message.info('Clicked cancel');
            }
        }
    }
</script>

<template id="subMain">
    <v-alert 
        color="red" 
        width="300" 
        max-height="200"
        border
        border-color="blue">
        color="red" 
        width="300" 
        max-height="200"
        border
        border-color="blue"
    </v-alert>

    <v-alert 
        width="300" 
        max-height="200"
        closable
        close-label="dsada"
        model-value
        v-model="alert">
        closable    
        v-model="alert"
    </v-alert>
    <button @click="alert=true;" style="width:200px; margin-bottom:10px; border-bottom:1px solid black"> closable alert 다시 키기</button>

    <v-alert 
        width="300" 
        max-height="200"
        elevation="24">
        elevation="24" *0~24의 숫자를 넣음    
    </v-alert>

    <v-alert 
        width="300" 
        max-height="200"
        location="dasdsa">   
        location
    </v-alert>
</template>
elevation
<script>
export default {
    name:'AlertComponent',
    data() {
        return {
            alert:true
        }
    },
}
</script>

<style scoped>
.v-alert {
    margin-bottom:20px;
}
</style>
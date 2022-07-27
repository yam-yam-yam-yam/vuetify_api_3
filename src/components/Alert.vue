<template id="subMain">
    <v-alert 
        color="red" 
        width="300" 
        min-height="250"
        border="end"
        border-color="blue">
        <p>color="red" </p>
        <p>width="300" </p>
        <p>min-height="250"</p>
        <p>border="end"</p>
        <p>border-color="blue"</p>
    </v-alert>

    <v-alert 
        width="300" 
        min-height="250"
        closable
        close-label="$vuetify.close"
        model-value
        v-model="alert">
        <p>closable</p>    
        <p>close-label="$vuetify.close" | aria-label임</p>
        <p>v-model="alert"</p>
    </v-alert>
    <button @click="alert=true;" style="width:250px; margin-bottom:10px; border-bottom:1px solid black"> closable alert 다시 키기</button>

    <v-alert 
        width="300" 
        min-height="250"
        elevation="24">
        <p>elevation="24" *0~24의 숫자를 넣음</p>
    </v-alert>

    <v-alert 
        width="300" 
        min-height="250"
        icon="mdi-domain"
        close-icon="mdi-arrow-up-bold-box-outline"
        closable>
        <p>icon="mdi-domain"</p>
        <p>close-icon="mdi-arrow-up-bold-box-outline"</p>
        <p>https://next.vuetifyjs.com/en/components/icons/ 에서 아이콘 보기</p>
    </v-alert>

    <v-alert 
        width="300" 
        min-height="250"
        icon="mdi-domain"
        close-icon="mdi-arrow-up-bold-box-outline"
        closable>
        <p>icon="mdi-domain"</p>
        <p>close-icon="mdi-arrow-up-bold-box-outline"</p>
        <p>https://next.vuetifyjs.com/en/components/icons/</p>
    </v-alert>

    <v-alert 
        width="300" 
        min-height="250"
        prominent
        icon="mdi-arrow-up-bold-box-outline">   
        <p>prominent | 중앙 큰 아이콘</p>
    </v-alert>

    <v-alert 
        width="300" 
        min-height="250"
        title="타이틀입니다"
        text="텍스트입니다">   
        <p>title="타이틀입니다"</p>
        <p>text="텍스트입니다"</p>
    </v-alert>

    <v-alert 
        type="info"
        width="300" 
        min-height="250">   
        type="info"
    </v-alert>

    <v-alert 
        width="300" 
        density="compact">   
        <p>density="compact"</p>
        <p>height 속성이 있으면 의미 없음</p>
    </v-alert>
    <v-alert 
        width="300" >   
        density속성이 없을때
    </v-alert>
    <v-alert 
        width="300" 
        density="comfortable">   
        <p>density="comfortable"</p>
        <p>height 속성이 있으면 의미 없음</p>
    </v-alert>

    <v-alert 
        width="300" 
        min-height="250"
        location="dasdsa"
        tag="span"
        theme="dark">   
        <p>tag="span" | 태그를 바꿔줌</p>
        <p>theme="dark"</p>
        <p>theme 설정은 https://next.vuetifyjs.com/en/features/theme/ 여기서 보기</p>
    </v-alert>

    <v-alert 
        width="300" 
        min-height="250"
        position="fixed"
        :rounded="'xl'"
        style="right:30px;">   
        <p>position="fixed"</p>
        <p>:rounded="'xl'"</p>
        <p>:rounded="true" 로도 가능</p>
    </v-alert>

    <v-alert 
        width="300" 
        min-height="250"
        variant="flat">   
        <p>variant="flat" (default)</p>
    </v-alert> 

    <v-alert 
        width="300" 
        min-height="250"
        variant="tonal">   
        <p>variant="tonal"</p>
    </v-alert>  

    <v-alert 
        width="300" 
        min-height="250"
        variant="elevated">   
        <p>variant="elevated"</p>
    </v-alert>  

    <v-alert 
        width="300" 
        min-height="250"
        variant="outlined">   
        <p>variant="outlined"</p>
    </v-alert>

    <v-alert 
        width="300" 
        min-height="250"
        variant="text">   
        <p>variant="text"</p>
    </v-alert>
    <v-alert 
        width="300" 
        min-height="250"
        variant="plain">   
        <p>variant="plain"</p>
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
<template src='./template.html'>
  
</template>

<script>
export default {
    data(){
        return{
            data:[
                {
                    content:'·品牌介紹'
                },
                {
                    content:'·選色系統'
                },
                {
                    content:'·產品介紹'
                },
                {
                    content:'·聯絡資訊'
                },
                {
                    content:'·共通任何裝置'
                },
            ]
        }
    },
    props: [
        'active'
    ],
    methods:{
        delayContent(index){
            if(this.active){
                return `animate__animated animate__flipInX animate__delay-0`+index+`s animate__slower':active`
            }
        }
    }

}
</script>

<style>

</style>
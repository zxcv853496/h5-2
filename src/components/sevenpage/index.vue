<template src='./template.html'>
  
</template>

<script>
export default {
    data(){
        return{
            data:[
                {
                    content:'·國家專利392項'
                },
                {
                    content:'·台灣金馬獎6項'
                },
                {
                    content:'·全球世界獎1項'
                },
                {
                    content:'·科技部專業領域獎5項'
                },
                {
                    content:'·其餘獎項25項'
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
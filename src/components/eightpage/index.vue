<template src='./template.html'>
  
</template>

<script>
export default {
    data(){
        return{
            data:[
                {
                    img:'/H5/2/img/eightpage/card-1.png',
                    content1:'競速車業',
                    content2:'黑黃設計'
                },
                {
                    img:'/H5/2/img/eightpage/card-2.png',
                    content1:'車次元',
                    content2:'霧感設計'
                },
                {
                    img:'/H5/2/img/eightpage/card-3.png',
                    content1:'李東根',
                    content2:'大理石設計'
                },
            ]
        }
    },
    props: [
        'active'
    ],
    methods:{
        deleayContent(index) {
            if(this.active){
                return `animate__animated animate__fadeIn animate__delay-00`+index+`s animate__slow':active}`
            }
        }
    }

}
</script>

<style>

</style>
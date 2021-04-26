<template src='./template.html'>
  
</template>

<script>
export default {
    data(){
        return{
            data:[
                {
                    img:'/H5/2/img/fivepage/2.jpg',
                    content1:'2000mAH',
                    content2:'持續使用20分'
                },
                {
                    img:'/H5/2/img/fivepage/2.jpg',
                    content1:'無限自由',
                    content2:'全屋無塵'
                },
                {
                    img:'/H5/2/img/fivepage/3.jpg',
                    content1:'智能感知',
                    content2:'重點清潔'
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
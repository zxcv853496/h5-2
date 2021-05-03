<template src='./template.html'>
  
</template>

<script>
export default {
    data(){
        return{
            img:[
                '/H5/2/img/ninepage/card1.png',
                '/H5/2/img/ninepage/card2.png',
                '/H5/2/img/ninepage/card3.png',
                '/H5/2/img/ninepage/card4.png',
                '/H5/2/img/ninepage/card5.png',
                '/H5/2/img/ninepage/card6.png',
                '/H5/2/img/ninepage/card7.png',
                '/H5/2/img/ninepage/card8.png',
                '/H5/2/img/ninepage/card9.png',
                '/H5/2/img/ninepage/card10.png',
                '/H5/2/img/ninepage/card11.png',
                '/H5/2/img/ninepage/card12.png',
                '/H5/2/img/ninepage/card13.png',
                '/H5/2/img/ninepage/card14.png',
                '/H5/2/img/ninepage/card15.png',
                '/H5/2/img/ninepage/card16.png',
                '/H5/2/img/ninepage/card17.png',
            ],
            hover:false
        }
    },
    props: [
        'active'
    ],
    methods:{
        mouseOver(){
            this.hover =! this.hover
        },
        mouseLeave(){
            this.hover=! this.hover
        }
    }
}
</script>

<style>

</style>
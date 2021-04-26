<template src='./template.html'>
  
</template>

<script>
export default {
    data() {
        return {
            timer:0,    
            mainpage:true,
        }
    },
    props: [
        'active'
    ],
    created () {
        this.timer = setInterval(this.mainBannerMove, 4000)
    },
    mounted() {
        this.mainBannerMove()
    },
    methods: {
        mainBannerMove() {
        this.mainpage =! this.mainpage
        },
    }

}
</script>

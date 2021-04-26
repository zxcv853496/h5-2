<template src='./template.html'>
  
</template>

<script>
export default {
    data(){
        return{
            data:[
                {
                    title:'2012年7月',
                    content:'公司正式成立'
                },
                {
                    title:'2013年3月',
                    content:'公司融資一百萬'
                },
                {
                    title:'2012年7月',
                    content:'公司獲得台灣企業獎'
                },
                {
                    title:'2012年7月',
                    content:'公司獲得台灣百強企業稱號'
                },
                {
                    title:'2012年7月',
                    content:'公司融資一百五十萬'
                },
                {
                    title:'2012年7月',
                    content:'平台用戶破千萬'
                },
            ]
        }
    },
    props: [
        'active'
    ],
}
</script>

<style>

</style>
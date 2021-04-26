<template src='./template.html'>
  
</template>

<script>
export default {
    data(){
        return{
            data:[
                {
                    name: "項目經理",
                    each: '3名',
                    pay: '10K-16K'
                },
                {
                    name: "諮詢顧問",
                    each: '5名',
                    pay: '10K-13K'
                },
                {
                    name: "軟體工程師",
                    each: '2名',
                    pay: '16K-26K'
                },
                {
                    name: "前端開發",
                    each: '3名',
                    pay: '10K-16K'
                },
                {
                    name: "日語翻譯",
                    each: '1名',
                    pay: '6K-10K'
                },
                {
                    name: "運營管理",
                    each: '1名',
                    pay: '8K-12K'
                },
                {
                    name: "營銷經理",
                    each: '1名',
                    pay: '10K-16K'
                },
                {
                    name: "市場專員",
                    each: '3名',
                    pay: '8K-12K'
                },
                {
                    name: "市場經理",
                    each: '1名',
                    pay: '10K-16K'
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
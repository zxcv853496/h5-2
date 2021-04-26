<template src='./template.html'>
  
</template>

<script>
export default {
    data(){
        return{
            options:[
                    "選擇職位",
                    "項目經理",
                    "諮詢顧問",
                    "軟體工程師",
                    "前端開發",
                    "日語翻譯",
                    "運營管理",
                    "營銷經理",
                    "市場專員",
                    "市場經理",
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
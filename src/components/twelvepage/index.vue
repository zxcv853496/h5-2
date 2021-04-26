<template src='./template.html'>
  
</template>

<script>
export default {
    data(){
        return{
            data:[
                {
                    title: '崗位職責:',
                    content:[
                        '負責完成產品H5，專題頁等線上運營設計',
                        '負責完成大促活動的主視覺設計及設計規範',
                        '能夠準確定位需求目標，快速輸出工作',
                    ]
                },
                {
                    title: '崗位要求:',
                    content:[
                        '本科及以上，3-5年工作經驗',
                        '善於溝通，學習能力強，對待工作有責任心',
                        '對用戶體驗有一定見解',
                        '對自己的產品有優秀的細節把控能力'
                    ]
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
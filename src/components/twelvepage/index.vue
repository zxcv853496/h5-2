<template src='./template.html'>
  
</template>

<script>
export default {
    data(){
        return{
            data:[
                {
                    title: '品牌設計:',
                    content:[
                        '以「市場設計」為核心並結合「視覺設計、數位體驗、包裝行銷」有效提升品牌競爭力與減少風險阻力。',
                    ]
                },
                {
                    title: '網站設計:',
                    content:[
                        '從網站洽詢、規劃、視覺設計、前後端程式設計、主機託管、網域申請等，一次到到位的服務。',
                    ]
                },
                {
                    title: '數位行銷:',
                    content:[
                        '消結合「品牌設計」與「市場設計」並精準投遞廣告讓品牌維持在一定熱度與品質。',
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
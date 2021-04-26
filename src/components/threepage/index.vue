<template src='./template.html'>
  
</template>

<script>
export default {
    data() {
        return{
            data:[
                {
                    img:'/H5/2/img/threepage/1.jpg',
                    title:'經營理念',
                    content:'引導成功的品牌舵手！游向設計的海洋 破開迎來的風浪 成就品牌的閃耀'
                },
                {
                    img:'/H5/2/img/threepage/2.jpg',
                    title:'企業精神',
                    content: '跨越變化莫測的海洋，才能到另一片大陸實踐夢想，找到耀眼的寶藏。 ',   
                },
                {
                    img:'/H5/2/img/threepage/3.jpg',
                    title:'企業願景',
                    content: '我們一起經歷的大風大浪與無數波折之後，在成為頂尖品牌的路上，看到的美麗與感動。', 
                }
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
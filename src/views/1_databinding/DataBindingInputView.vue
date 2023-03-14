<template>
    <div>
        <input type="text" v-model="userId"/>
    </div>
</template>
<script>
export default { 
    components:{},
    data() {
        return{
           userId: 'Ddongs'  //v-model 로 태그속성을 지정해주면 해당 input태그 벨류값으로 자동으로 데이터바인딩됨. 
        }   //브라우저 쪽에서 수정을 하게되면 자동적으로 js에도 업데이트됨=> 뷰의 가장 큰 장점 양방향 데이터 바인딩.
    },
    setup(){},
    created(){},
    mounted(){},
    unmounted(){},
    methods:{}
}
</script>
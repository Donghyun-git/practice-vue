<template>
    <div>
        <input type="text" v-model="userId"/>
        <button @click="myFunction"> 클릭</button> <!--onclick 대신 @click function-->
        <button @click="changeData"> 변경</button>
        <br>
        <input type="text" v-model="num1" />+
        <input type="text" v-model="num2" />=
        <span>{{ num1 + num2 }}</span>
        <br>
        <input type="text" v-model.number="num3" />+
        <input type="text" v-model.number="num4" />=   <!--v-model . number 을 사용하면 알아서 형변환 해줌... 와...-->
        <span>{{ num3 + num4 }}</span>
    </div>
</template>
<script>
export default {   
    components:{},
    data() {
        return{
           userId: 'Ddongs',//v-model 로 태그속성을 지정해주면 해당 input태그 벨류값으로 자동으로 데이터바인딩됨. 브라우저 쪽에서 수정을 하게되면 자동적으로 js에도 업데이트됨=> 뷰의 가장 큰 장점 양방향 데이터 바인딩.
           num1: 0,  
           num2: 0,
           num3: 0,
           num4: 0
        }
    },
    setup(){},
    created(){},
    mounted(){},
    unmounted(){},
    methods:{
        myFunction(){
            console.log(this.userId)   // 여기에 있는 모든 함수들은 vue 객체에 저장된다. this는 vue 객체의 모든 것을 가리킨다. => 따라서 this.userId로 data 접근 가능.
        },
        changeData(){
            this.userId = "Jeremy";   //와....진짜 신세계네....
        }
    }
}

</script>


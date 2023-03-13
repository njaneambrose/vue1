
<template>
    <div class="form">
        <p v-if="isdsb">Hide text</p>
        <input type="number" placeholder="Enter number a" v-model.number="a"/>
        <input type="number" placeholder="Enter number b" v-model.number="b"/>
        <h4 :class="cl">{{  a + b }}</h4>
        <p>Clicks = {{ count }}</p>
        <button v-if="isdsb" @click=add()>Click Me</button>
    </div>
</template>

<script>

export default{
    name: 'SimpleCalc',
    props: {
        hi: String,
        cl: String,
        isdsb: Boolean
    },
    data(){
        return {
            a: 0,
            b: 0,
            count: 0
        }
    },
    methods: {
        add() {
            this.count++;
        }
    }
}

</script>
<style scoped>
 input{
    box-shadow: 0 2px 4px 0 rgba(0,0,0,.2);
    height: 23px;
 }
</style>
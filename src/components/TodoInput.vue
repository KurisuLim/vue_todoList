<template>
    <div>
        <input 
        type="text"
        class="input"
        placeholder="New Todo"
        v-model="inputEntry"
        required
        />
        <button
        class="btn"
        @click="submitEvent(inputEntry)"
        >
        Submit
        </button>
        <p style="color: red; font-size: 13px;" v-if="error">
            You must enter something first!
        </p>
    </div>
</template>

<script>
export default {
    name: 'TodoInput',
    data(){
        return{
            inputEntry: '',
            error: false
        }
    },
    methods: {
        submitEvent (todoListDetail){
            if(todoListDetail === '') return this.error = true;
            console.log(this.inputEntry)
        }
    }
}
</script>
//scoped means this style only exist in this component
<style lang="scss" scoped>
@import '../../public/variables.scss/variables.scss';

.input{
    width: 100%;
    padding: 8px 10px;
    border: 1px solid $vue-blue;
}
.btn{
    margin: 10px auto;
    padding: 5px 10%;
    border: 1px solid $vue-blue;
}

</style>


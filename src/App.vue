<style lang="scss">
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
    }
</style>

<template>
    <div id="app">
        <input
            type="text"
            v-model="inputValue">
        </input>
        <input
            @click="handleClick"
            type="button"
            :value="outStr">
        </input>
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';
    import Component from 'vue-class-component';

    @Component({})
    export default class App extends Vue {
        private outStr: string = '外部字符串';
        private inputValue: string = '';
        public handleClick() {
            // console.log(this.outStr);
        }
        public created() {
            // console.log(2);
        }
        public mounted() {
            // console.log(1);
        }
    }
</script>

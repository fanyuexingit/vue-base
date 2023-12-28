<template>

    <h3>class</h3>
    
    <p :style="{color: activeColor, fontSize: fontSize + 'px'}">s11111</p>
    
    <p :style="styleObject">s2222222222</p>
    </template>
    
    
    <script>
    export default {
        data() {
            return {
                activeColor: "green",
                fontSize: 30,
                styleObject: {
                    color: "red",
                    fontSize: "30px"
                }
               
            }
        }
    }
    
    </script>
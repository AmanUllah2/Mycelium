<template>
    <!-- For Small screens -->
    <div>
           
           <img class="button" src="../assets/Button.png" alt="">
           <img class="balloon" src="../assets/balloon.png" alt="">
    </div>
</template>

<style scoped>
.balloon{
    height: 500px;
    width: 700px;
    position: absolute;
    margin-left: -100px;
    margin-top: 60px;
}
.balloon:hover {
    -ms-transform: scale(1.2); /* IE 9 */
    -webkit-transform: scale(1.2); /* Safari 3-8 */
    transform: scale(1.2); 
    }
.button{
    position: absolute;
    margin-left: -710px;
    margin-top: 60px;
}   
.button:hover {
    -ms-transform: scale(1.1); /* IE 9 */
    -webkit-transform: scale(1.1); /* Safari 3-8 */
    transform: scale(1.1); 
    }
</style>
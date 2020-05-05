<template>
<div class="ima">
<!-- For Small screens -->   
    <div class=".d-none .d-sm-block d-lg-none">
    <xs/>
    </div>
<!-- For Large screens -->
<div class="container cap d-none d-md-none d-lg-block">
    <div>
    <!-- <img width="400px" class="stem" src="../assets/stem.png" /> -->
    <!-- <img height="400px" width="400px" src="../assets/capfill.png" alt=""> -->
    </div>
    <div class="parent">
    <img v-show="cap" id="capfillmove" width="400px" class="yet-another-over" src="../assets/capfill.png" />
    <img v-show="balloon" class="balloon" src="../assets/balloon.png" alt="">
    <img v-show="b1" class="bubblexs" src="../assets/Bubble.png" alt="">
    <img v-show="b2" class="bubblemd" src="../assets/Bubble.png" alt="">
    <img v-show="b3" class="bubblelg" src="../assets/Bubble.png" alt="">
    <!-- <img v-show="b3" class="shadow" src="../assets/Shadow.png" alt=""> -->
    <img v-show="Button" class="buttonHome" src="../assets/Button.png" alt="">
    <img v-show="stem" width="400px" class="another-over" src="../assets/stem.png" />
    <img v-show="soil" height="300px" width="400px" src="../assets/soil.png" class="over-img"/>
    <img v-show="roots" width="400px" class="rootimg" src="../assets/roots.png" />
    </div>
</div>

</div>
</template>

<script>
import xs from '../components/missionsx'
export default {
    data(){
        return{
            cap: false,
            balloon: false,
            b1: false,
            b2: false,
            b3: false,
            Button: false,
            stem: false,
            soil: false,
            roots: false
        }
    },
    components:{
        xs
    },
    created(){
      setTimeout(()=> this.roots = true, 1000)
      setTimeout(()=> this.soil = true, 1500),
      setTimeout(()=> this.stem = true, 2000),
      setTimeout(()=> this.cap = true, 2500),
      setTimeout(()=> this.b1 = true, 3000),
      setTimeout(()=> this.b2 = true, 3300),
      setTimeout(()=> this.b3 = true, 3600),
      setTimeout(()=> this.balloon = true, 4100),
      setTimeout(()=> this.Button = true, 4300)
    }
}
</script>

<style scoped>
    .shadow{
        position: absolute;
        margin-left: 130px;
        margin-top: 130px;
    }
    .buttonHome{
    position: absolute;
    margin-left: 850px;
    height: 950px;
    width: 1300px;
    margin-top: 400px;
    }
    .buttonHome:hover {
    -ms-transform: scale(1.2); /* IE 9 */
    -webkit-transform: scale(1.2); /* Safari 3-8 */
    transform: scale(1.2); 
    }
    .bubblelg{
    position: absolute;
    margin-left: 550px;
    height: 120px;
    width: 220px;
    margin-top: 200px;
    }
    .bubblelg:hover {
    -ms-transform: scale(1.2); /* IE 9 */
    -webkit-transform: scale(1.2); /* Safari 3-8 */
    transform: scale(1.2); 
    }
    .bubblemd{
    position: absolute;
    margin-left: 460px;
    height: 100px;
    width: 190px;
    margin-top: 170px;
    }
    .bubblemd:hover {
    -ms-transform: scale(1.2); /* IE 9 */
    -webkit-transform: scale(1.2); /* Safari 3-8 */
    transform: scale(1.2); 
    }
    .bubblexs{
        position: absolute;
        margin-left: 390px;
        height: 80px;
        width: 150px;
        margin-top: 150px;
    }
    .bubblexs:hover {
    -ms-transform: scale(1.2); /* IE 9 */
    -webkit-transform: scale(1.2); /* Safari 3-8 */
    transform: scale(1.2); 
    }
    .balloon{
        position: absolute;
        width: 1340px;
        height: 740px;
        margin-left: 350px;
        margin-top: 120px;
    }
    .balloon:hover {
    -ms-transform: scale(1.2); /* IE 9 */
    -webkit-transform: scale(1.2); /* Safari 3-8 */
    transform: scale(1.2); 
    }
    #capfillmove{
    animation: shake 0.5s;
    animation-iteration-count: infinite;
    }
    @keyframes shake {
    0% { transform: translate(1px, 1px) rotate(0deg); }
    }
    .cap{
        margin-top:35px;
        margin-left:200px ;
    }
    .parent{
    position: relative;
    }
    .rootimg{
    margin-top: 805px;
    }
    .over-img{
    position: absolute;
    left: 0;
    margin-left: 0px;
    margin-top:620px;
    }
    .another-over{
    position: absolute;
    margin-top: 60px;
    }
    .yet-another-over{
        position: absolute;
        margin-top: 20px;
    }

    .ima{
    margin-top: -35px;
    background-image: url('../assets/background.png');    
    margin-right: -500px;
    }
</style>
<template>
  <section>
    <ul class="box-area">
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
    </ul>

    <div class="box">
        <div class="circle">
            <h2>
                Season's <br/> Greetings
            </h2>
        </div>
    </div>
</section>

</template>

<script>
export default {
  name: 'Season'
}
</script>
  
 

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


section {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 100vh;
    background: linear-gradient(to left, #8942a8, #ba382f);
    overflow: hidden;
}   

section .box-area {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100vh;
    overflow: hidden;
}

section .box-area li {
    position: absolute;
    display: block;
    list-style: none;
    width: 25px;
    height: 25px;
    background: rgba(255, 255, 255, 0.2);
    animation: animate 20s linear infinite;
    border-radius: 100%;
    bottom: -150px;
}

section .box-area li:nth-child(1){
    left: 26%;
    width: 80px;
    height: 80px;
    animation-delay: 0s;
}
section .box-area li:nth-child(2){
    left: 12%;
    width: 80px;
    height: 80px;
    animation-delay: 1.5s;
    animation-duration: 10s;
}
section .box-area li:nth-child(3){
    left: 70%;
    width: 100px;
    height: 100px;
    animation-delay: 0s;
    animation-duration: 5.5s;
}
section .box-area li:nth-child(3){
    left: 68%;
    width: 100px;
    height: 100px;
    animation-delay: 0s;
    animation-duration: 5.5s;
}
section .box-area li:nth-child(4){
    left: 32%;
    width: 150px;
    height: 150px;
    animation-delay: 0s;
    animation-duration: 15s;
}
section .box-area li:nth-child(5){
    left: 50%;
    width: 100px;
    height: 100px;
    animation-delay: .5s;
    animation-duration: 5.5s;
}    
section .box-area li:nth-child(6){
    left: 50%;
    width: 110px;
    height: 110px;
     animation-delay: 1.5s;
    animation-duration: 10s;
}    
section .box-area li:nth-child(7){
    left: 0%;
    width: 110px;
    height: 110px;
     animation-delay: .5s;
    animation-duration: 5.5s;
}    
section .box-area li:nth-child(8){
    left: 75%;
    width: 110px;
    height: 110px;
      animation-delay: 1.5s;
    animation-duration: 15s;
}    
section .box-area li:nth-child(9){
    left: 90%;
    width: 110px;
    height: 110px;
    animation-delay: 0s;
}    
section .box-area li:nth-child(10){
    left: 5%;
    width: 110px;
    height: 110px;
    animation-delay: 3.5s;
}    

@keyframes animate {
    0%{
        transform: translateY(0) rotate(0deg);
        opacity: 1;
    }
    100%{
        transform: translateY(-800px) rotate(360deg);
        opacity: 0;
    }
}


section .box {
    position: absolute;
    width: 450px;
    height: 450px;
}

section .box::before {
    content: '';
    position: absolute;
    top: 0;
    left: 50%;
    width: 100%;
    height: 100%;
    background: linear-gradient(to right,rgb(255, 255, 255),transparent);
    opacity: 0.1;
    transform: rotate(45deg);
    transform-origin: left;
    border-radius: 100%;
}
section .box .circle{
    position: relative;
    width: 100%;
    height: 100%;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.152), #e4e3e857);
     display: flex;
    align-items: center;
    justify-content: center;
    text-transform: capitalize;
    border-radius: 50%;
    z-index: 1;
}

section .box .circle::before{
    content: '';
    position: absolute;
    top: 5px;
    left: 5px;
    right: 5px;
    bottom: 5px;
    background: linear-gradient(315deg, rgba(255, 255, 255, 0.234), #e4e3e852);
    border-radius: 50%;
}

section .box .circle h2 {
    position: absolute;
    z-index: 2;
    font-size: 4em;
    color:#f5f5fa;
    text-align: center;
    text-shadow: 0 0 0 #ba382f57;
}



@media only screen and (max-width: 550px){

    section {
        width: 100%;
        height: 100vh;
        overflow-x: hidden;
    }   
  
    
  
    section .box .circle h2 {
        font-size: 3em;
        
    }
   

    section .box {
          width: 330px;
        height: 330px;
        overflow: hidden;
     }   
  

}
          
        
</style>

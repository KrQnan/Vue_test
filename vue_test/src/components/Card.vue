<script>
import { ref } from "vue";
</script>

<template>
        <div id="card">
            <h1>Random object</h1>
            <img src="https://picsum.photos/200/300?random=10" alt="">
            <div class="overlay">
                <h5 id="text">Check this</h5>
            </div>
        </div>
</template>

<style>
#card{
    position: relative;
    width:18rem
    
}
#card img{
    width: 100%;
    height: auto;
}

.overlay{
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    height: 100%;
    width: 100%;
    opacity: 0;
    transition: .5s ease;
    background-color: rgba(176, 177, 169, 0.5);
}
#card:hover .overlay{
    opacity: 1
}

#card:hover{
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    opacity: 0.5;
    transition: .9s ease;
    background-color: rgba(176, 177, 169, 0.5);
}


#text{
    color: white;
    font-size: 20px;
    position: absolute;
    top: 50%;
    left: 50%;
    -webkit-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    text-align: center;
}


</style>
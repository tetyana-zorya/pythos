<template>
  <div style="padding:1em;" id="whole">
      <img @click="begin()" width="100%" id="fp" style="position:relative; bottom:300px;"  src="@/assets/AP3.png">
      
      <div class="welcome-position">
        <!-- <div id="enter">
         <v-btn @click="begin()">Enter</v-btn>

        </div> -->
        <div class="welcome-text" id="auth">
        Authentic To You.
        </div>
        <div id="rella">
          Rella.
        </div>
        <div id="create">
          create your dream wedding
          <a href="#"><v-icon style="color:#212121" x-large>mdi-arrow-right</v-icon></a>
        </div>
      </div>
      
    
    

  </div>
</template>

<script>

  //import Welcome from '../components/Welcome'

  export default {
    name: 'Home',

    components: {
    },
    created() {
     
    },
    methods: {

      begin() {
        this.start()
       

        setTimeout(function () {
            document.getElementById('fp').style.opacity = 0;
            }, 5000);

        setTimeout(function () {
            let ele = document.getElementById('auth')
            ele.classList.add('appear');
            }, 1000);
        setTimeout(function () {
            let ele = document.getElementById('auth')
            ele.classList.add('disappear');
            }, 2000);

        setTimeout(function () {
            document.getElementById('whole').style.backgroundColor = '#EEE5E9';
            document.getElementById('whole').style.transition = 'background-color 1s ease';
            }, 3000);

        setTimeout(function () {
          let elem = document.getElementById('rella')
          elem.classList.add('appear');
            }, 4000);
        
        setTimeout(function () {
          let elem = document.getElementById('create')
          elem.classList.add('appear');
            }, 4500);
        
        setTimeout(function () {
          let elem = document.getElementById('rella')
          elem.style.opacity = 1;
            }, 5000);

        setTimeout(function () {
          let elem = document.getElementById('create')
          elem.style.opacity = 1;
            }, 5500);
      },

      start: function() {
        const element = document.getElementById('fp')
        element.classList.add('flower');
      },

    }
  }
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Stoke:wght@300&display=swap');

a {
  text-decoration: none;
}
  .welcome-position {
    text-align: center;
    margin: auto;
    
  }
  .welcome-text {
    font-size:50px;
    font-family: 'Stoke', serif;
    position: absolute;
    top:400px;
    left:37%;
  }
  #enter {
    font-size:50px;
    font-family: 'Stoke', serif;
    position: absolute;
    top:300px;
    left:48%;
    z-index: 1000;
  }

  #auth {
    opacity: 0;
  }
  #rella {
    font-size:150px;
    font-family: 'Stoke', serif;
    position: absolute;
    top:260px;
    left:38%;
    opacity: 0;
  }

  #create {
    font-size:50px;
    font-family: 'Stoke', serif;
    position: absolute;
    top:460px;
    left:30%;
    opacity: 0;
  }

  .flower {
    animation: move 5s;
    animation-timing-function: ease-out;
  }

  .appear {
    animation: fadein 2s;
    animation-timing-function: ease-in-out;
  }
  .disappear {
    animation: fadeout 2s;
    animation-timing-function: ease-in-out;
  }
 

@keyframes move {
  from {
    top:-300px; opacity: 1;
  }
  
  to {
    top:-600px; opacity: .1;
    
  }
}

@keyframes fadein {
  from {
    opacity: 0;
  }
  
  to {
    opacity: 1;
    
  }
}
@keyframes fadeout {
  from {
    opacity: 1;
  }
  
  to {
    opacity: 0;
    
  }
}

</style>

<svelte:head>
    <link rel="stylesheet" type='text/css' href="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/devicon.min.css" />
</svelte:head>
<h1 id="title">My Tech Stacks</h1>
<div class="Marquee">
    <div class="Marquee-content">
      <div class="Marquee-tag">
        <i class="devicon-svelte-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-javascript-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-php-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-tensorflow-original"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-googlecloud-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-linux-plain"></i>
      </div>
      
      <div class="Marquee-tag">
        <i class="devicon-react-original"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-express-original"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-go-original-wordmark"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-c-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-figma-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-arduino-plain"></i>
      </div>
        <div class="Marquee-tag">
      <i class="devicon-mongodb-plain"></i>
      </div>
    </div>
</div>
<h1 id="tagline">You Name It, I've Built It</h1>
<div class="hidden"><p>I'm always ready to take on new challenges and explore the latest trends in tech. You name it, I've built it – and I'm excited to bring that experience to your next project.</p></div>
<div class="Marquee">
    <div class="Marquee-content-rev">
      <div class="Marquee-tag">
        <i class="devicon-svelte-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-javascript-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-php-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-tensorflow-original"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-googlecloud-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-linux-plain"></i>
      </div>
      
      <div class="Marquee-tag">
        <i class="devicon-react-original"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-express-original"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-go-original-wordmark"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-c-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-figma-plain"></i>
      </div>
      <div class="Marquee-tag">
        <i class="devicon-arduino-plain"></i>
      </div>
        <div class="Marquee-tag">
      <i class="devicon-mongodb-plain"></i>
      </div>
    </div>
</div>
<style>
    h1 {
        margin: 20px;
    }
    #title::after {
        content: '';
        display: block;
        width: 100px;
        height: 1px;
        background: white;
        margin: 10px 0;
    }
    #tagline {
        margin-top: 50px;
        font-family: 'satoshi-regular',sans-serif;
        font-size: 4rem;
        display: flex;
        justify-content: center;
    }
    #tagline:hover + .hidden {
        opacity: 1;
        transition: all 0.5s ease-in-out;
    }
    .hidden {
        color: white;
        text-align: center;
        /* width: 80%; */
        font-family: 'satoshi-light',sans-serif;
        font-size: 1rem;
        display: flex;
        justify-content: center;
        align-items: center;
        opacity: 0;
        transition: all 0.5s ease-in-out;
    }
    .hidden p {
        width: 80%;
    }
    .Marquee {
  /* background: -webkit-linear-gradient(225deg, #008ed9, #8b00db);
  background: -moz-linear-gradient(225deg, #008ed9, #8b00db);
  background: -o-linear-gradient(225deg, #008ed9, #8b00db);
  background: -ms-linear-gradient(225deg, #008ed9, #8b00db);
  background: linear-gradient(-135deg, #008ed9, #8b00db); */
  /* background: rgb(244 240 255/0.5); */
  width: 100vw;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
  /* padding: 1em; */
  color: #fff;
  font-weight: 200;
  display: -webkit-box;
  display: -moz-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: box;
  display: flex;
  -webkit-box-align: center;
  -moz-box-align: center;
  -o-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center;
  overflow: hidden;
  height: 250px;
}
.Marquee-content {
  display: -webkit-box;
  display: -moz-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: box;
  display: flex;
  animation: marquee 18s linear infinite running;
}
.Marquee-content-rev {
  display: -webkit-box;
  display: -moz-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: box;
  display: flex;
  animation: marquee-reverse 18s linear infinite running;
}
.Marquee-content-rev:hover {
  -webkit-animation-play-state: paused;
  -moz-animation-play-state: paused;
  -o-animation-play-state: paused;
  -ms-animation-play-state: paused;
  animation-play-state: paused;
}
.Marquee-content:hover {
  -webkit-animation-play-state: paused;
  -moz-animation-play-state: paused;
  -o-animation-play-state: paused;
  -ms-animation-play-state: paused;
  animation-play-state: paused;
}
.Marquee-tag {
  width: 200px;
  height: 200px;
  margin: 0 0.1em;
  font-size: 100px;
  padding: 0.5em;
  /* background: rgba(255,255,255,0.4); */
  background: rgba( 255, 255, 255, 0.25 );
/* box-shadow: 0 8px 32px 0 rgba(255, 255, 255, 0.37); */
box-shadow: 0 3px 7px 0px rgba(255, 255, 255, 0.37);
backdrop-filter: blur( 4px );
-webkit-backdrop-filter: blur( 4px );
border-radius: 10px;
  transition: all 0.2s ease;
}
.Marquee-tag:hover {
  background: rgba(255,255,255,0.5);
  -webkit-transform: scale(1.1);
  -moz-transform: scale(1.1);
  -o-transform: scale(1.1);
  -ms-transform: scale(1.1);
  transform: scale(1.1);
  cursor: pointer;
}
@keyframes marquee {
  0% {
    -webkit-transform: translateX(0);
    -moz-transform: translateX(0);
    -o-transform: translateX(0);
    -ms-transform: translateX(0);
    transform: translateX(0);
  }
  100% {
    -webkit-transform: translate(-50%);
    -moz-transform: translate(-50%);
    -o-transform: translate(-50%);
    -ms-transform: translate(-50%);
    transform: translate(-50%);
  }
}
@keyframes marquee-reverse {
    0% {
        -webkit-transform: translate(-50%);
        -moz-transform: translate(-50%);
        -o-transform: translate(-50%);
        -ms-transform: translate(-50%);
        transform: translate(-50%);
    }
    100% {
        -webkit-transform: translateX(0);
        -moz-transform: translateX(0);
        -o-transform: translateX(0);
        -ms-transform: translateX(0);
        transform: translateX(0);
    }
}
@media (max-width: 768px){
    .Marquee-tag {
        width: 100px;
        height: 100px;
        font-size: 50px;
    }
    .hidden{
        font-size: 0.7rem;
    }
    .Marquee {
        height: 150px;
    }
}

</style>
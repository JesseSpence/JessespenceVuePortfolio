<template>
    <section id="projects">
    
            <h1 class="section-heading mb-5">Projects</h1>
        
        <div class="container d-flex justify-content-center">
            
        <ul class="nav nav-pills mb-3" id="pills-tab" role="tablist">
            <li class="nav-item" role="presentation">
              <div class="cubelinks active" id="pills-home-tab" data-bs-toggle="pill" data-bs-target="#pills-home" type="button" role="tab" aria-controls="pills-home" aria-selected="true"><div class="cube">
                <div class="top"><i class="fa-solid my-2 ms-3 h3 text-light fa-arrow-pointer"></i></div>
                <div class="right"></div>
                <div class="bottom"></div>
                <div class="left"></div>
                <div class="back"></div>
                <div class="front"></div>
              </div></div>
            </li>
            <li class="nav-item" role="presentation">
              <div class="cubelinks " id="pills-profile-tab" data-bs-toggle="pill" data-bs-target="#pills-profile" type="button" role="tab" aria-controls="pills-profile" aria-selected="false">
                  <div class="cube">
                <div class="top"><i class="fa-solid my-2 ms-3 h3 text-light fa-arrow-pointer"></i></div>
                <div class="right"></div>
                <div class="bottom"></div>
                <div class="left"></div>
                <div class="back"></div>
                <div class="front"></div>
              </div></div>
            </li>
            <li class="nav-item" role="presentation">
              <div class="cubelinks" id="pills-contact-tab" data-bs-toggle="pill" data-bs-target="#pills-contact" type="button" role="tab" aria-controls="pills-contact" aria-selected="false"><div class="cube">
                <div class="top"><i class="fa-solid my-2 ms-3 h3 text-light fa-arrow-pointer"></i></div>
                <div class="right"></div>
                <div class="bottom"></div>
                <div class="left"></div>
                <div class="back"></div>
                <div class="front"></div>
              </div></div>
            </li>
          </ul>
        </div>
        
        <div class="row">
          <div class="tab-content" id="pills-tabContent">

            <div class="tab-pane fade show active" id="pills-home" role="tabpanel" aria-labelledby="pills-home-tab">

                 <div id="body" class=" d-flex justify-content-around flex-wrap">
    <div v-for="project of projects" :key="project.title">
      <div class="project-card mb-5">
        <div id="projects" class="card col-lg-4" style="width: 290px">
          <img :src="project.img" />
          <h5 class="sub-heading mb-3">{{ project.title }}</h5>
         <p class="card-text">{{ project.description }}</p>
         <div class="as" >
           <a :href="project.github"><i class="fa-solid fa-horse-head ps-5"></i> GitHub</a>
          <a :href="project.netlify"><i class="fa-solid fa-horse-head ps-5"></i> Netlify</a>
          </div>
        </div>
      </div>
      </div>
    </div>
            </div>
        
            <div class="tab-pane fade" id="pills-profile" role="tabpanel" aria-labelledby="pills-profile-tab">
                ..
            </div>
            

             <div class="tab-pane fade" id="pills-contact" role="tabpanel" aria-labelledby="pills-contact-tab">
                ..
            </div>
          </div>
          </div>

</section>
	
		
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
        'img': 'https://picsum.photos/id/238/200/300 ',
        'title': 'Calculator',
        'github': 'https://github.com/JesseSpence/Calculator',
        'netlify': 'https://rad-piroshki-9acc5b.netlify.app',
        'description': 'Simple JavaScript Calculator',
      },
       {
        'img': 'https://picsum.photos/id/238/200/300 ',
        'title': 'More Calculators',
        'github': 'https://github.com/JesseSpence/More-calculators',
        'netlify': 'https://shiny-kulfi-edb6be.netlify.app',
        'description': 'BMI calculator with a temperature convertor using JavaScript',
        },
       {
        'img': 'https://picsum.photos/id/238/200/300 ',
        'title': 'Resturant company',
        'github': 'https://github.com/JesseSpence/Delicious-WebDesign',
        'netlify': 'https://musical-kheer-4ea418.netlify.app',
        'description': 'A prototype for a resturant website',
        },
       {
        'img': 'https://picsum.photos/id/238/200/300 ',
        'title': 'Real Estate Company',
        'github': 'https://github.com/JesseSpence/Real-Estate-Update',
        'netlify': 'https://profound-figolla-aa3d5c.netlify.app',
        'description': 'A prototype for a Real-estate website',
        },
       {
        'img': 'https://picsum.photos/id/238/200/300 ',
        'title': 'Gaming Store',
        'github': 'https://github.com/JesseSpence/ljmaUpdated',
        'netlify': 'https://ljma-games-online-store.netlify.app',
        'description': 'A prototype for a Gamestore Webite',
        },
       {
        'img': 'https://picsum.photos/id/238/200/300 ',
        'title': 'Holiday Destination',
        'github': 'github.com/JesseSpence/branchestask',
        'netlify': 'https://app.netlify.com/sites/lovely-choux-ac0aa1/overview',
        'description': 'A Little Project learning HTML and CSS',
        },
      {
        'img': 'https://picsum.photos/id/238/200/300 ',
        'title': 'To-Do list',
        'github': 'https://github.com/JesseSpence/Bootstrap-practise',
        'netlify': 'https://sparkling-sunshine-70a2fc.netlify.app',
        'description': 'A simple to-Do list App',
        },
      {
        'img': 'https://picsum.photos/id/238/200/300 ',
        'title': 'Basic developer portfolio',
        'github': 'https://github.com/JesseSpence/Bootstrap-practise',
        'netlify': 'https://graceful-lebkuchen-0994af.netlify.app',
        'description': 'A simple to-Do list App',
      },
]
    };
  },
}
</script>

<style scoped>
#body{
margin:3%;
padding:2rem;
}
img{
height:250px;
}
.card{
 background:var(--text-mute);
 box-shadow: 1px 1px 8px 8px  var(--el-color);
  animation: shadow linear infinite 2s;
  height:401px;
  padding:1.5%;
 }
 p{
  background:rgba(0, 0, 0, 0.093);
 }
 .as{
  position:absolute;
  bottom:10px;
 }
 a{
  text-decoration:none;
  color:var(--el-color) !important;
 }
.cube { padding-right:100px;
    width: 50px;
    height: 50px;
    position: relative;
    transform-style: preserve-3d;
    transform: rotateX(-20deg) rotateY(-45deg); 
 }
 .cube div {
    width: 50px;
    height: 50px;
    position: absolute;
    background: var(--el-color);

    box-shadow: inset 0px 0px 30px rgba(0, 0, 0, 0.6);
 }
 .cube:hover .top {
    transform: translateX(-60px);
 }
 
 
 .cube div.top {
    z-index: 1000;
    transform: rotateX(90deg);
    margin-top: -25px;
    transition: all ease-in-out 1s;
 }
 .cube div.top:hover{
     transform: translateX(-60px);
 }
 
 .cube div.right {
    transform: rotateY(90deg); 
    margin-left: 25px;
    transition:all ease-in-out 1s;
 }
 .cube div.right:hover, .top {
    display:block;
 }
 

 .cube div.bottom {
   transform: rotateX(90deg);
   margin-top: 25px;
 }
 
 .cube div.left {
    transform: rotateY(-90deg);
    margin-left: -25px;
 }
 
 .cube div.front {
    transform: translateZ(25px); 
    transition: all ease-in-out 2s;
 }
 
 .cube div.back {
    transform: translateZ(-25px); 
 }

 @media screen and (max-width:390px) {
    .cube { 
        width: 25px;
        padding-right: 60px;
     }
    
     .cube div { 
        width: 25px;
        height: 25px;

     }
     .cube div.top {
        transform: rotateX(90deg);
        margin-top: -12px;
        transition: all ease-in-out 1s;
     }
     .cube div.top:hover{
         transform: translateX(-60px);
     }
     
     .cube div.right {
        transform: rotateY(90deg); 
        margin-left: 12px;
        transition:all ease-in-out 1s;
     }
     
     
    
     .cube div.bottom {
       transform: rotateX(90deg);
       margin-top: 12.5px;
     }
     
     .cube div.left {
        transform: rotateY(-90deg);
        margin-left: -12.5px;
     }
     
     .cube div.front {
        transform: translateZ(12.5px); 
        transition: all ease-in-out 2s;
     }
     
     .cube div.back {
        transform: translateZ(-12.5px); 
     }
    
 }
 #projects{
     min-height: fit-content;
     padding-top: 5%;
    padding-bottom: 5%;
    max-width:100vw;
 }
 
</style>

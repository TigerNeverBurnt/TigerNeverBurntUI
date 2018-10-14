<template>

  <div id="app">

          <el-header class=level2 id=example3>
            Tiger Hacka!
          </el-header>

    <el-container style="height:700px; border: 1px solid #eee">
      
      <el-aside width="300px" style="background-color: rgb(238, 241, 246)">
    <sd/>  <sd/><sd/><sd/><sd/>  <sd/>
    

  </el-aside>
          
            <el-container>

              <el-main style="background-color: rgb(238, 241, 246)">
                  <div>
                      <Record ref="record"></Record>
                  </div>
                  <br><br>               

                  <div class=textround>
                    <InputField/>
                  </div>
              </el-main> 
            </el-container>
            
              
          

    </el-container>
    <!-- <el-footer style="margin-bottom:0px; height:100%">Footer
                        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d99296.49783267855!2d-92.4010505011079!3d38.94647296871662!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x87dcb79505ed8739%3A0xc18305329c07fb48!2sUniversity+of+Missouri!5e0!3m2!1sen!2sus!4v1537897164099" width="100%" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
            </el-footer> -->
            
  </div>
</template>

<script>

import InputField from './InputField.vue';
import Record from './Record.vue';
import sd from './sd.vue';
export default {
  components:{
    InputField,Record,sd
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Josefin+Sans');
@font-face {
  src: url('./Georgia Bold Italic.ttf') format('opentype');
  font-family: myFirstFont;
}
#app {
  
  font-family: myFirstFont;
  
  font: italic;
  text-align: center;
  
}
.el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 100%;
  }
.type1 {
    width: 2%;
    height:2%;
    text-align: center;
    border-radius: 50%;
    border: 2px solid black;
}
 .el-header, .el-footer {
    font-family: 'Josefin Sans', sans-serif;
    text-align: center;
    line-height: 20px;
  }
  body > .el-container {
    margin-bottom: 40px;
  }
  .level2{
    /* background-image:url("./Atlas.jpg"); */
    text-align: center;
    
    font-size: 40px;
    margin: 0;
    line-height: 60px;
    color: #2d9fcc;
    
    -webkit-margin-before: 0em;
    -webkit-margin-after: 0em;
    -webkit-margin-start: 0px;
    -webkit-margin-end: 0px;
    font-weight: bold;
}
  .textround{ background: #aee6de; border:1px solid #accdd9; padding:6px;
	
	/* ROUNDED CORNERS */
	-webkit-border-radius: 5px;
	-moz-border-radius: 5px;
	-ms-border-radius: 5px;
	-o-border-radius: 5px;
	border-radius: 5px;

	/* SHADOWS */
	-webkit-box-shadow:inset 0px 0px 5px 0px #9fc7d6;
	-moz-box-shadow:inset 0px 0px 5px 0px #9fc7d6;
	-ms-box-shadow:inset 0px 0px 5px 0px #9fc7d6;
	-o-box-shadow:inset 0px 0px 5px 0px #9fc7d6;
	box-shadow:inset 0px 0px 5px 0px #9fc7d6;

  }
  .div .textround{ margin:0 0 -3px;

	/* ROUNDED CORNERS */
	-webkit-border-radius: 0px;
	-moz-border-radius: 0px;
	-ms-border-radius: 0px;
	-o-border-radius: 0px;
	border-radius: 0px;

  }
  #example1 {
    
    background-color: silver;
    background-image: radial-gradient(circle at 100% 150%, silver 24%, white 25%, white 28%, silver 29%, silver 36%, white 36%, white 40%, transparent 40%, transparent), radial-gradient(circle at 0 150%, silver 24%, white 25%, white 28%, silver 29%, silver 36%, white 36%, white 40%, transparent 40%, transparent), radial-gradient(circle at 50% 100%, white 10%, silver 11%, silver 23%, white 24%, white 30%, silver 31%, silver 43%, white 44%, white 50%, silver 51%, silver 63%, white 64%, white 71%, transparent 71%, transparent), radial-gradient(circle at 100% 50%, white 5%, silver 6%, silver 15%, white 16%, white 20%, silver 21%, silver 30%, white 31%, white 35%, silver 36%, silver 45%, white 46%, white 49%, transparent 50%, transparent), radial-gradient(circle at 0 50%, white 5%, silver 6%, silver 15%, white 16%, white 20%, silver 21%, silver 30%, white 31%, white 35%, silver 36%, silver 45%, white 46%, white 49%, transparent 50%, transparent);
    background-size: 100px 50px;
  }
  #example2{
    background-color: #556;
    background-image: linear-gradient(30deg, #445 12%, transparent 12.5%, transparent 87%, #445 87.5%, #445), linear-gradient(150deg, #445 12%, transparent 12.5%, transparent 87%, #445 87.5%, #445), linear-gradient(30deg, #445 12%, transparent 12.5%, transparent 87%, #445 87.5%, #445), linear-gradient(150deg, #445 12%, transparent 12.5%, transparent 87%, #445 87.5%, #445), linear-gradient(60deg, #99a 25%, transparent 25.5%, transparent 75%, #99a 75%, #99a), linear-gradient(60deg, #99a 25%, transparent 25.5%, transparent 75%, #99a 75%, #99a);
    background-size: 80px 140px;
    background-position: 0 0, 0 0, 40px 70px, 40px 70px, 0 0, 40px 70px;
  }
  #example3{
    background: #acb6e5;  /* fallback for old browsers */
    background: -webkit-linear-gradient(to right, #86fde8, #acb6e5);  /* Chrome 10-25, Safari 5.1-6 */
    background: linear-gradient(to right, #86fde8, #acb6e5); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

  }
</style>
    


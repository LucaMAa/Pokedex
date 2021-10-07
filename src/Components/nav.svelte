
    <div class="BtnCartoon">
        <li><a href="/">Pokedex</a></li>
      </div>
      <div class="BtnCartoon">
        <li><a href="/about">What is a Pokedex?</a></li>
      </div>

<style>

.BtnCartoon{
    position:relative;
    display:inline-block;
    margin:20px;
    justify-content: right;
    
  }
  
  .BtnCartoon li{
    padding-top: 40px;
    color:white;
    font-family:Helvetica, sans-serif;
    font-weight:bold;
    font-size:20px;
    text-align: center;
    text-decoration:none;
    background-color:#3b00dd;
    display:block;
    position:relative;
    padding:10px 40px;
    
    -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
    text-shadow: 0px 1px 0px #000;
    filter: dropshadow(color#0000);
    
    -webkit-box-shadow:inset 0 1px 0 #FFE5C4, 0 10px 0 #22027c;
    -moz-box-shadow:inset 0 1px 0 #FFE5C4, 0 10px 0 #22027c;
    box-shadow:inset 0 1px 0 #FFE5C4, 0 10px 0 #22027c;
    
    -webkit-border-radius: 5px;
    -moz-border-radius: 5px;
    border-radius: 5px;
  }
  
  .BtnCartoon li:active{
    top:10px;
    background-color:#3b00dd;
    
    -webkit-box-shadow:inset 0 1px 0 #FFE5C4, inset 0 -3px 0 #22027c;
    -moz-box-shadow:inset 0 1px 0 #FFE5C4, inset 0 -3pxpx 0 #22027c;
    box-shadow:inset 0 1px 0 #FFE5C4, inset 0 -3px 0 #22027c;
  }
  
  .BtnCartoon:after{
    content:"";
    height:100%;
    width:100%;
    padding:4px;
    position: absolute;
    bottom:-15px;
    left:-4px;
    z-index:-1;
    background-color:#2B1800;
    -webkit-border-radius: 5px;
    -moz-border-radius: 5px;
    border-radius: 5px;
  }
    
</style>
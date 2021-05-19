## Udemy course 

### CSS TRICKS 

- pour mettre des images à la même taille, il vaut mieux mettre une div sur l'élément puis dans le CSS mettre background-img:url(nom.png) avec tout les background-position etc. 
- pseudo element ::before & after, il faut mettre un content: "" pour créer le bloc puis rajouter les attributs qu'on veut 
- z index doesn't work with default position it has to be relative, fixed or absolute position element

### JQuery function 

- appear and disappear menu code : 
````
in JS file 

     $(function() {
         var box = $('.box');
         var button = $('.open-menu, .header-menu');
         button.on('click', function(){
           box.toggleClass('active');
         });
       });
       
 in HTML file 
 
   <div class="box">
        <div class="container">
            <div class="header-menu">
              <button><img src="http://www.i2symbol.com/images/symbols/check/multiplication_x_u2715_icon_256x256.png"></button>
            </div>
                <ul class="top-menu">
                          <li class="menu-items"><a href="#">Inbox</a></li>
                          <li class="menu-items"><a href="#">Files</a></li>
                          <li class="menu-items"><a href="#">Notifications</a></li>
                          <li class="menu-items twitter"><a href="https://twitter.com/juwanpetty">Say 👋 on Twitter</a></li>
                </ul>
            
                <ul class="bottom-menu">
                <li class="bottom-menu-item"></li>
                </ul>
        </div>
    </div>

    <div class="open-menu">
        <button><img src="https://cdn4.iconfinder.com/data/icons/wirecons-free-vector-icons/32/menu-alt-256.png"></button>
    </div>
    
  
    <h1 class="text">A menu will slide over from the left.</h1> 
    
in CSS file 

.box {
    height: 100vh;
    width: 300px;
    position: absolute;
    left: -350px;
    z-index: 1001;
    background: pink;
    overflow: hidden;
    text-align: left;
  -webkit-transition: -webkit-transform 250ms ease-in-out;
  transition: transform 250ms ease-in-out;
}
    
.active {

    transform: translateX(350px);
    box-shadow: 0 19px 38px rgba(0,0,0,0.30), 0 15px 12px rgba(0,0,0,0.22);
} 

.open-menu {
    display: inline-block;
}

.header-menu {
    height: 50px;
    background: pink;
	margin-bottom: 200px
}

````



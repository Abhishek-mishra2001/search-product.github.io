<!DOCTYPE html>
<html>
  <head>
    <title>Search Product List</title>
    <style>
      * {
  padding: 0;
  margin: 0;
  position: relative;
  box-sizing: border-box;
}

.listing-section {
  width: 100%;
  float: left;
  padding: 1%;
  border-bottom: 0.01em solid #dddbdb;
}

.product {
  float: left;
  width: 23%;
  border-radius: 2%;
  margin: 1%;
}

.product:hover {
  box-shadow: 1.5px 1.5px 2.5px 3px rgba(0, 0, 0, 0.4);
  -webkit-box-shadow: 1.5px 1.5px 2.5px 3px rgba(0, 0, 0, 0.4);  
  -moz-box-shadow:    1.5px 1.5px 2.5px 3px rgba(0, 0, 0, 0.4);
}

.image-box {
  width: 100%;
  overflow: hidden;
  border-radius: 2% 2% 0 0;
}

.images {
  height: 15em;
  background-size: cover; 
  background-position: center center; 
  background-repeat: no-repeat;
  border-radius: 2% 2% 0 0;
  transition: all 1s ease;
  -moz-transition: all 1s ease;
  -ms-transition: all 1s ease;
  -webkit-transition: all 1s ease;
  -o-transition: all 1s ease;
}

.images:hover {
  transform: scale(1.2);
  overflow: hidden;
  border-radius: 2%;
}

/* IMAGES */
#image-1 {background-image: url("https://sc01.alicdn.com/kf/UT8.CaXX2NXXXagOFbXC/fresh-navel-oranges.jpg");}

#image-2 {background-image: url("https://newenglandapples.files.wordpress.com/2014/10/img_5595.jpg")}

#image-3 {background-image: url("https://sc01.alicdn.com/kf/UT8ovSIXQNaXXagOFbXt/Fresh-Passion-Fruit-with-Best-Price-and.jpg")}

#image-4 {background-image: url("http://www.foodmatters.com/media/images/articles/16-powerful-reasons-to-eat-pineapple.jpg")}

#image-5 {background-image: url("http://membrillo.com.au/wp-content/uploads/2016/11/bg-mango-01.jpg")}

#image-6 {background-image: url("http://ell.h-cdn.co/assets/16/27/980x490/landscape-1467750721-gettyimages-146896572.jpg")}

#image-7 {background-image: url("https://media.istockphoto.com/id/173242750/photo/banana-bunch.jpg?s=612x612&w=0&k=20&c=MAc8AXVz5KxwWeEmh75WwH6j_HouRczBFAhulLAtRUU=")}

#image-8 {background-image: url("https://media.istockphoto.com/id/1343635919/photo/delicious-ripe-plums-on-white.jpg?b=1&s=170667a&w=0&k=20&c=XeWD1KfuYw-8Sem8tb4YKtRoAet1w51yeCP-qtQx728=")}

#image-9 {background-image: url("https://thumbs.dreamstime.com/b/avocado-18188183.jpg")}

#image-10 {background-image: url("https://www.parhlo.com/wp-content/uploads/2016/04/Valencia_market_-_lemons-1940x1454.jpg")}


#image-11 {background-image: url("https://cdn.britannica.com/01/140601-050-8DE3378E/jujube-tree.jpg")}
#image-12 {background-image: url("https://health.clevelandclinic.org/wp-content/uploads/sites/3/2020/12/eatJackfruit-823672534-770x533-1.jpg")}

.text-box {
  width: 100%;
  float: left;
  border: 0.01em solid #dddbdb;
  border-radius: 0 0 2% 2%;
  padding: 1em;
}

h2, h3 {
  float: left;
  font-family: 'Roboto', sans-serif;
  font-weight: 400;
  font-size: 1em;
  text-transform: uppercase;
  margin: 0.2em auto;
}

.item, .price {
  clear: left;
  width: 100%;
  text-align: center;
}

.price {
  color: Grey;
}

.description, label, input {
  float: left;
  clear: left;
  width: 100%;
  font-family: 'Roboto', sans-serif;
  font-weight: 300;
  font-size: 1em;
  text-align: center;
  margin: 0.2em auto;
}

input:focus {
  outline-color: #fdf;
}

label {
  width: 60%;
}

.text-box input {
  width: 15%;
  clear: none;
}


  input{
  
    margin: 10px;
    height: 31px;
    border: 2px solid black;
  }
  form{
    width: 50%;
    margin: 0 auto;
  }
    </style>
    
  </head>
  <body>
    <div>
      <form>
        <input type="text" name="" placeholder="Search Product" id="search-item" onkeyup="search()" />
      </form>
    </div>
    <div class="listing-section" id="product-list" >
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-1"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Orange</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious oranges!</p>
        </div>
      </div>
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-2"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Apple</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious apples!</p>
        </div>
      </div>
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-3"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Passionfruit</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious passionfruit!</p>
        </div>
      </div>
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-4"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Pineapple</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious pineapples!</p>
        </div>
      </div>
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-5"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Mango</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious mangos!</p>
        </div>
      </div>
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-6"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Coconut</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious coconuts!</p>
        </div>
      </div>
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-7"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Banana</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious bananas!</p>
        </div>
      </div>
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-8"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Plum</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious plums!</p>
        </div>
      </div>
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-9"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Avocado</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious avocados!</p>
        </div>
      </div>
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-10"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Lemon</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious lemons!</p>
        </div>
      </div>
      
      
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-11"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Jujube</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious Jujube!</p>
        </div>
      </div>
      <div class="product">
        <div class="image-box">
          <div class="images" id="image-12"></div>
        </div>
        <div class="text-box">
          <h2 class="item">Jackfruit</h2>
          <h3 class="price">$4.99</h3>
          <p class="description">A bag of delicious Jackfruits!</p>
        </div>
      </div>
    </div>
  </body>
  <script>
    "use strict";
  const search = ()=>{
    const searchBox = document.getElementById('search-item').value.toUpperCase();
    const product = document.querySelectorAll('.text-box');
    const pname = document.getElementsByTagName('h2');
    const noFound = document.querySelector('#noFound');
      for(var i = 0; i < pname.length; i++){
          let match = product[i].getElementsByTagName('h2')[0];
          if(match){
              let textValue = match.textContent || match.innerHTML;
              if(textValue.toUpperCase().indexOf(searchBox) > -1){
                  product[i].parentElement.style.display = "";
              }else{
                product[i].parentElement.style.display = "none";
                
              }
          }
         
      }
  }

   
        
// 0-100 5/unit     100*5 500   
// 101-200 10/unit  100*10 1000
// 201-300 15/unit  100*15 1500
// 300+    20/unit  80*20 1600
    //380 unit = 4600 rs 

    function getUnit(num){
        
          if(num > 300){
                var unitVal = new Array(4).fill(num);
             const arrVal1 =   unitVal[0]/num*100*5;
             const arrVal2 =   unitVal[1]/num*100*10;
             const arrVal3 =   unitVal[2]/num*100*15;
             const arrVal4 =  (unitVal[3] - 300)*20;
                 const finalVal = arrVal1 + arrVal2 + arrVal3 + arrVal4; 
                return finalVal;
          }else if(num<200){
              var unitVal = new Array(3).fill(num);
              const arrVal1 =   unitVal[0]/num*100*5;
             const arrVal2 =   unitVal[1]/num*100*10;
             const arrVal3 =   (unitVal[2] - 200)*15;
            
                 const finalVal = arrVal1 + arrVal2 + arrVal3; 
                return finalVal;
              
          }
        
        
        
    }

     console.log(getUnit(230))

        function UnitCount(num){
           if (num < 500){
            let unit = num/5;
            return unit;
           }else if(num > 500 && num <= 1500){
                let subUnit = (num - 500)/10;
               let unit = subUnit + 100;
              return unit;
           }else if(num > 1500 && num <= 3000){
            let subUnit = (num - 1500)/15;
               let unit = subUnit + 200;
              return unit;
              
           }else{
            let subUnit = (num - 3000)/20;
               let unit = subUnit + 300;
              return unit;
           }

        }
        console.log(UnitCount(8000));
  </script>
</html>


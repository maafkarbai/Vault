#  After school Activities app
- Don't use Defensive, BI names
- Use sort
	- Use multiple sorts 
		- Subject
		- Location
		- Price (Ascending/ Descending)
		- Availability
- Shopping cart 
- Checkout (Disabled by default until something is added)
	- Name and Phone at checkout as well (Compulsory and it should be added to checkout) also add validation
- Order placed screen 
- Search functionality 
	- Should Display Items searched
- Your inventory should be 10 items and max 5 at a time in cart 

# v-text
- Retrieves data from the data { Key:"Data"  } and puts it in 
```javascript
<p v-text:"NameofKeyInsideData"></p>
```

# v-bind
- Used to binding html attributes like src for img tag
```javascript
<img v-bind:src="Product.image">
```

# v-html (Not recommended)
- Used to render html code
```javascript
      <p v-html="product.description"></p>
         let App = new Vue({
        el:"#app",
        data:{    
          sitename:"Vue.Js Pet Depot",
          product:{
            id:1001,
            title:"Cat Food, 25lb bag",
            description:"A 25 Pounds Bag of <em>irresistible</em>," + "Organic Goodness for Your Cat",
            price:2000,
            image:"Images/Catfood.png"
          }
        }
    })
```

# Adding Array to data in VUE Instance
```javascript
   let App = new Vue({
      el: "#app",
      data: {
        sitename: "Vue.Js Pet Depot",
        product: {
          id: 1001,
          title: "Cat Food, 25lb bag",
          description:
            "A 25 Pounds Bag of <em>irresistible</em>," +
            "Organic Goodness for Your Cat",
          price: 2000,
          image: "Images/Catfood.png",
        },
        cart: [],
      },
    });
```

# v-on Directive 
- Executes functions with Events 

# Computed Property
- Calculates using available info
- Like calculating age from 
- Cannot have parameters only methods can
- Line execution Sequence matters for values

```javascript


    let App = new Vue({
		data:{
			var1:12
			var2:13
		}
      methods: {
        addToCart: function () {
			this.var1
			this.var2 
			//this will take values from upward variables in data
        },
		
      },

    }
    });
```

# v-show
- Takes binary values
- toggles display to show or not
- -If the condition is `true`, Vue sets `display: block` (or the default display value of the element).
- If the condition is `false`, Vue sets `display: none`, hiding the element but keeping it in the DOM
```javascript
<div v-show="isVisible"> This element is conditionally visible. </div>
```

# v-if
- Takes cases for if statements
```javascript
//Yes Case (show button)
<button v-on:click="addToCart" v-if="canAddToCart">Add to Cart</button>
//If Not Case ()
<button disabled="disabled" v-else>Add to Cart</button>
```


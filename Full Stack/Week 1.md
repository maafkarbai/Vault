- Stacks 
- What is x in stack?
- what's the stack you use (MEVN)
- tryhackme 
- What is CDN (content delivery network, these are interconnected servers)? 
- What is Mount?
- what is el? 
	- Links the vue to div
	- Keyword for element (type id="#app")
- What is a data keyword?
	- It takes key value pairs and displays the value for the key?

- Eloquent JS
- What is onclick()?
- createelement()?
- .innertext?
- AppendChild()
- .value?
``` 
const inputElement = document.getElementById('nameInput');
const value = inputElement.value; // Get the value
inputElement.value = 'New Value'; // Set a new 
```


## - intializing vue
	let app = new Vue({
		el: "#DivID",	
		data: { newTask: ' ' }
		methods: {
		methodname: {
			//logic
		}
		}
	})
	


- Two way Binding?
- v-model:
	- Dynamic 
	- lets say 
	`<input type="text" v-model="newTask">`  The value is stored in newTask Variable and vue processes it 
	
- v-on
	- Event Listener?
	- example: v-on:click="functionname / methoddefinedintheinitializationveyvaluepair"

- Methods in vuejs?
	methods: {
		additem: function(){
			//logic
		}
	}
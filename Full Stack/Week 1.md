
---

### Stacks

- **What is 'x' in a stack?**: 'x' typically refers to an element being pushed or popped from the stack.
- **Stack You Use (MEVN)**: MongoDB, Express.js, Vue.js, Node.js.

---

### TryHackMe

- **Definition**: A platform offering cybersecurity learning and practical hands-on exercises.

---

### CDN (Content Delivery Network)

- **Definition**: Interconnected servers distributed globally to deliver content faster and improve website performance.

---

### Mount

- **Definition**: In Vue.js, "mount" refers to attaching the Vue instance to a specific DOM element.

---

### el in Vue.js

- **Definition**:
    - Links the Vue instance to the specified DOM element.
    - **Example**: `el: "#app"` targets the element with ID `#app`.

---

### Data Keyword in Vue.js

- **Definition**:
    - Holds key-value pairs for reactive data.
    - **Example**: `{ key: 'value' }`.

---

### Eloquent JavaScript Concepts

#### onclick()

- **Definition**: An HTML event attribute to trigger a JavaScript function when an element is clicked.

#### createElement()

- **Definition**: Creates a new HTML element dynamically.
    - **Example**: `document.createElement('div')`.

#### .innerText

- **Definition**: Sets or gets the text content of an element.
    - **Example**: `element.innerText = 'Hello World';`.

#### appendChild()

- **Definition**: Appends a child element to a parent element.
    - **Example**: `parent.appendChild(child)`.

#### .value

- **Definition**: Gets or sets the value of an input element.
    - **Example**:
        
        ```javascript
        const inputElement = document.getElementById('nameInput');
        const value = inputElement.value; // Get the value
        inputElement.value = 'New Value'; // Set a new value
        ```
        

---

### Initializing Vue.js

- **Example**:
    
    ```javascript
    let app = new Vue({
      el: "#DivID",
      data: { newTask: '' },
      methods: {
        methodName: function () {
          // logic
        }
      }
    });
    ```
    

---

### Two-Way Binding

- **Definition**: Automatically synchronizes data between the DOM and the Vue instance.
- **Key Directive**: `v-model`.
    - **Example**: `<input type="text" v-model="newTask">` stores input value in `newTask`.

---
### v-on

- **Definition**: Event listener directive in Vue.js.
- **Example**: `v-on:click="methodName"` triggers a method when clicked.

---

### Methods in Vue.js

- **Definition**: Functions declared inside the `methods` object for logic handling.
- **Example**:
    
    ```javascript
    methods: {
      addItem: function () {
        // logic
      }
    }
    ```
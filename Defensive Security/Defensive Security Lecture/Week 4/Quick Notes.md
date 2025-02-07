```javascript
<input type="text" v-model="order.firstname" /> 
```
take the input and put it in the order array's firstname  

# v-for


## .trim
- Trims off white space
```javascript
   <p>
            <strong>First Name:</strong>
            <input
              v-model.trim="order.firstName"
              type="text"
              v-model="order.firstName"
            />
          </p>
```

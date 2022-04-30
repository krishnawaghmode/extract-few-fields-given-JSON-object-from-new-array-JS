# How can you extract a few fields from the given JSON object and from a new array?
 
## We will need to use the map() method, we will pass the element and then return only the required key from that element

<!-- <details><summary><b>Answer</b></summary> -->

  ```javascript
const input = {


	"students": [
        {
        	name:"Rahul",
        	email:"rahul@gmail.com",
        	id:1
        },
        {
        	name:"Ganesh",
        	email:"ganesh@gmail.com",
        	id:2
        },
        {
        	name:"Atish",
        	email:"atish@gmail.com",
        	id:3
        },
        {
        	name:"Manoj",
        	email:"manoj@gmail.com",
        	id:4
        },



	]
}

const output = input.students.map(function(item) {

	let stdObj = {
		name: item.name,
		email: item.email,
	}

	return stdObj;
})

console.log(output)

//output
/*
[
    {
        "name": "Rahul",
        "email": "rahul@gmail.com"
    },
    {
        "name": "Ganesh",
        "email": "ganesh@gmail.com"
    },
    {
        "name": "Atish",
        "email": "atish@gmail.com"
    },
    {
        "name": "Manoj",
        "email": "manoj@gmail.com"
    }
]
*/
```
<!-- </details> -->

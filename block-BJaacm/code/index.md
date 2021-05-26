```js
let user = {
  name: 'Arya',
  sibling: ['Robb', 'Ryan', 'John'],
};
let allBrothers = ['Robb', 'Ryan', 'John'];
let brothersCopy = user.sibling;
let usename = user.name;
let newUser = user;
```

1. Memory representation

- Create the memory representation of the above snippet on notebook.
- Take a photo/screenshot and add it to the folder `code`

!(./hello.jpg) 

2. Answer the following with reason:

- `user == newUser;` // true - the contents of the user was copied by reference from the new user so both are equal.
- `user === newUser;` // true - since all the values are copied exactly in the newUser so both are strictly equal
- `user.name === newUser.name;` //  true - all the values of user and newUser are same
- `user.name == newUser.name;` true
- `user.sibling == newUser.sibling;` // true
- `user.sibling === newUser.sibling;` // true
- `user.sibling == allBrothers;` // false
- `user.sibling === allBrothers;` // false
- `brothersCopy === allBrothers;` // false
- `brothersCopy == allBrothers;` // false
- `brothersCopy == user.sibling;` //  true
- `brothersCopy === user.sibling;` // true 
- `brothersCopy[0] === user.sibling[0];` // true
- `brothersCopy[1] === user.sibling[1];` // true
- `user.sibling[1] === newUser.sibling[1];` // true

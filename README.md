# Mock test

## Using jsonplaceholder.typicode.com

### Listing all resources

```javascript
fetch('https://my-json-server.typicode.com/sfeuga/mock/update_focus_skills')
  .then((response) => response.json())
  .then((json) => console.log(json));
```

### Creating a resource

```javascript
fetch('https://my-json-server.typicode.com/sfeuga/mock/update_focus_skills', {
  method: 'POST',
  body: JSON.stringify({
    user_id: 'a7fff30d-5aae-40af-a631-fe2a2b082d0f',
    skills: ["Python", "Machine Learning", "Data Analysis"]
  }),
  headers: {
    'Content-type': 'application/json',
  },
})
  .then((response) => response.json())
  .then((json) => console.log(json));
```

Output:

```javascript
{
  id: 1234
  user_id: 'a7fff30d-5aae-40af-a631-fe2a2b082d0f',
  skills: [
    'Data Analysis',
    'Machine Learning',
    'Python'
  ]
}
```

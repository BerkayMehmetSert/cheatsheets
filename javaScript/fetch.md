<h1 style="font-family: Roboto" align="center">
FETCH CHEAT SHEET 
</h1>

<h3 style="font-family: Roboto">
Fetch
</h3>

```javascript
fetch('/data.json')
  .then(response => response.json())
  .then(data => {
    console.log(data)
  })
  .catch(err => ...) 
```

<h3 style="font-family: Roboto">
Response 
</h3>

```javascript
fetch('/data.json')
.then(res => {
  res.text()       // response body (=> Promise)
  res.json()       // parse via JSON (=> Promise)
  res.status       //=> 200
  res.statusText   //=> 'OK'
  res.redirected   //=> false
  res.ok           //=> true
  res.url          //=> 'http://site.com/data.json'
  res.type         //=> 'basic'
                   //   ('cors' 'default' 'error'
                   //    'opaque' 'opaqueredirect')

  res.headers.get('Content-Type')
})
```

<h3 style="font-family: Roboto">
Request Options 
</h3>

```javascript
fetch('/data.json', {
  method: 'post',
  body: new FormData(form), // post body
  body: JSON.stringify(...),

  headers: {
    'Accept': 'application/json'
  },

  credentials: 'same-origin', // send cookies
  credentials: 'include',     // send cookies, even in CORS

}) 
```

<h3 style="font-family: Roboto">
Catching Errors
</h3>

```javascript
etch('/data.json')
  .then(checkStatus)
function checkStatus (res) {
  if (res.status >= 200 && res.status < 300) {
    return res
  } else {
    let err = new Error(res.statusText)
    err.response = res
    throw err
  }
}
```

<h3 style="font-family: Roboto">
Using with node.js 
</h3>

```javascript
const fetch = require('isomorphic-fetch') 
```
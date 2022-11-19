# This is my README.md file
#### Here you can find some examples of my javascript codes

[<img src="https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png" width="200"/>](https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png)

Projects:
  * AJAX
  ```javascript
  let xhr = new XMLHttpRequest();
xhr.open("GET", "https://mdn.github.io/learning-area/javascript/oojs/json/superheroes.json");
xhr.send();
xhr.onload = function(){}
```

  * AJAX in JQuery
```javascript
$.ajax('https://api.github.com/users/' + username.toLowerCase(),{
	dataType: 'json',
	data: {},
	success: function(result){
		console.log(result);
		$('.userImg').attr('src', result['avatar_url']);
		$('.username').html(result['name']);
		$('.userURL').attr('href', result['html_url']);
		$('.userURL').show();
	},
	error: function(xhr){
		console.log(xhr.statusText)
	}
	});
});
```
[link on my github](https://github.com/theantonyis)

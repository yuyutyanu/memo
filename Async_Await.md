Async/Await

```
function sleep(delay){
	return new Promise((resolve,reject)=>{
		setTimeout(function(){resolve(delay)},delay)
	})
}

async function exec(){
	var a = await sleep(500)
	console.log(a)
	var b = await sleep(100)
	console.log(b)
}

exec()

//500
//100
```


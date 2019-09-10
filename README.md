# trycatch
Custom tryCatch Function


```javascript
function tryCatch(tryFn,catchFn=()=>{}){
	try{
		return tryFn();
	}catch(er){
		return catchFn(er);
	}
}


let x = tryCatch(_=> a.b.c.d, _=> defaultValue);
```


```js
function miniMaxSum(arr) {
	let max = arr[0]
	let min = arr[0]
	let sum = arr[0]
	
	for(let i = 1; i < arr.length; i++) {
		sum += arr[i]
		if(arr[i] < min) {
			min = arr[i]
		}else if (arr[i] > max) {
			max = arr[i]
		}
	}
	
	console.log(sum - max, sum - min)
}
```
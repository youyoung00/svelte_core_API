<script>
	let name = 'SHIN'
	let fruits = ['Apple', 'Banana', 'Cherry']
	let user = {
		name: 'SHIN',
		depth: {
		  a: 'b'	
		},
		numbers: [1,2]
	}

	let numbers = user.numbers
	let hello = 'world'

	function assign(){
		// let hello = 'world' // script탑레벨이 아닌 블럭내에 선언된 변수는 반응성을 가질 수 없음
		name = 'Neo'
		// fruits.push('Orange')
		// fruits = fruits
		fruits = [...fruits, 'Orange']
		// user.name = 'Neo'
		// user.depth.a = 'c'

		// await tick() 과 같은 비동기로 push()가 동작. 
		// user 자체가 갱신되기 때문에 push(3)dl 동작함.
		user.numbers.push(3)

		numbers = numbers
	}
</script>

<button on:click={assign}>Assign! </button>
<h2>name: {name}</h2>
<h2>fruits: {fruits}</h2>
<h2>user name: {user.name}</h2>
<h2>user depth a: {user.depth.a}</h2>
<h2>user numbers: {user.numbers}</h2>
<h2>numbers: {numbers}</h2>
<h2>{hello}</h2>
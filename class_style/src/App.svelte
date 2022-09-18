<script>
	let active = false
</script>

<button on:click={() => {active = !active}}>
	Toggle!
</button>

<!-- <div class={active ? 'active' : ''}> -->
<div class:hello={active}>
	Hello
</div>

<style>
	div {
		width: 120px;
		height: 200px;
		background: royalblue;
		border-radius: 10px;
		display: flex;
		justify-content: center;
		align-items: center;
		color: white;
		transition: .4s;
	}
	.hello{
		width: 250px;
		background: tomato;
	}
</style>
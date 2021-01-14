<script>
    export let name = 'Steve Jobs';
</script>

<div class="input">
    <input type="text" bind:value={name}>
    <p>Hello {name}!</p>
</div>